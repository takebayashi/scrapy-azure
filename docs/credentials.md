# Credentials

`scrapy-azure` uses [azure-identity](https://pypi.org/project/azure-identity/) and relies on the behavior of [DefaultAzureCredential](https://learn.microsoft.com/en-us/python/api/overview/azure/identity-readme?view=azure-python#defaultazurecredential).

## Using Azure managed identities

You can use [Azure managed identities](https://learn.microsoft.com/en-us/entra/identity/managed-identities-azure-resources/overview).

- If you use system-assigned managed identities, no configuration is required.

- If you use user-assigned managed identities, the environment variable `AZURE_CLIENT_ID` must be set to the client ID.
