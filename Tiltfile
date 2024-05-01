LOCAL_PATH = os.getenv("LOCAL_PATH", default='.')
NAMESPACE = os.getenv("NAMESPACE", default='default')
WAIT_TIMEOUT = os.getenv("WAIT_TIMEOUT", default='10m00s')
TYPE = os.getenv("TYPE", default='web')

k8s_custom_deploy(
    'my-web-app-axl',
    apply_cmd="tanzu apps workload apply -f config/workload.yaml --update-strategy replace --debug --live-update" +
               " --local-path " + LOCAL_PATH +
               " --namespace " + NAMESPACE +
               " --wait-timeout " + WAIT_TIMEOUT +
               " --type " + TYPE +
               " --yes --output yaml",
    delete_cmd="tanzu apps workload delete -f config/workload.yaml --namespace " + NAMESPACE + " --yes",
    container_selector='workload',

    # Live Update IntelliJ:
    deps=['build.gradle.kts', './build/classes/java/main', './build/resources/main'],
    live_update=[
       sync('./build/classes/java/main', '/workspace/BOOT-INF/classes'),
       sync('./build/resources/main', '/workspace/BOOT-INF/classes')
    ]
)

k8s_resource('my-web-app-axl', port_forwards=["8080:8080"],
            extra_pod_selectors=[{'carto.run/workload-name': 'my-web-app-axl', 'app.kubernetes.io/component': 'run'}])
