A function app runs on a specific version of the Azure Functions runtime. There are two major versions: 1.x and 2.x. By default, function apps that are created version 2.x of the runtime. This article explains how to configure a function app in Azure to run on the version you choose.


Azure Functions lets you target a specific version of the runtime by using the FUNCTIONS_EXTENSION_VERSION application setting in a function app. The function app is kept on the specified major version until you explicitly choose to move to a new version.