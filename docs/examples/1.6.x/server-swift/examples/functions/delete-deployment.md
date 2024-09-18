import Appwrite

let client = Client()
    .setEndpoint("https://cloud.appwrite.io/v1") // Your API Endpoint
    .setProject("<YOUR_PROJECT_ID>") // Your project ID
    .setKey("<YOUR_API_KEY>") // Your secret API key

let functions = Functions(client)

let result = try await functions.deleteDeployment(
    functionId: "<FUNCTION_ID>",
    deploymentId: "<DEPLOYMENT_ID>"
)
