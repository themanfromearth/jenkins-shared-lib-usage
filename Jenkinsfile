@Library(["jenkins-shared"]) _

def deployments = [
    dev: [
        [ cluster: "dev", environment: "develop", serviceName: "checkout-snapshots-api-v1", instances: 1 ],
        [ cluster: "dev", environment: "develop", serviceName: "checkout-snapshots-api-v1-pt", instances: 1 ],
        [ cluster: "staging", environment: "develop", serviceName: "checkout-snapshots-api-v1-develop", instances: 3 ]
    ]
]

apiPipeline(param: "merhaba", param2: "ali", deployments: deployments)