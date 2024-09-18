from appwrite.client import Client

client = Client()
client.set_endpoint('https://cloud.appwrite.io/v1') # Your API Endpoint
client.set_project('<YOUR_PROJECT_ID>') # Your project ID
client.set_session('') # The user session to authenticate with

databases = Databases(client)

result = databases.create_document(
    database_id = '<DATABASE_ID>',
    collection_id = '<COLLECTION_ID>',
    document_id = '<DOCUMENT_ID>',
    data = {},
    permissions = ["read("any")"] # optional
)