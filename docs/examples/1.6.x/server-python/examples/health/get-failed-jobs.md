from appwrite.client import Client
from appwrite.enums import 

client = Client()
client.set_endpoint('https://cloud.appwrite.io/v1') # Your API Endpoint
client.set_project('<YOUR_PROJECT_ID>') # Your project ID
client.set_key('<YOUR_API_KEY>') # Your secret API key

health = Health(client)

result = health.get_failed_jobs(
    name = .V1_DATABASE,
    threshold = None # optional
)