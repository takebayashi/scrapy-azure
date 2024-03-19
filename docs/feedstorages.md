# Feed storage backends

## Azure BLOB Storage

To enable the Azure BLOB Storage backend, set `FEED_STORAGES` in `settings.py` as follows:

```python
FEED_STORAGES = {"wasbs": "scrapy_azure.feedstorage.AzureBlobFeedStorage"}
```

Then set `FEEDS` as follows:

```python
FEEDS = {
    "wasbs://myaccount.blob.core.windows.net/mycontainer/myblob": {
        "format": "jsonl",
        "overwrite": True,
    }
}
```
