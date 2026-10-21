boolean disableIndexTriggers = env.BRANCH_NAME != 'main'

quadletPipeline(
    disableIndexTriggers: disableIndexTriggers,
    podmanSecretMappings: [
        [
            type: 'usernamePassword',
            credentialsId: 'mqtt',
            podmanSecretPasswordName: 'mqtt_password',
            podmanSecretUsernameName: 'mqtt_username'
        ]
    ]
)
