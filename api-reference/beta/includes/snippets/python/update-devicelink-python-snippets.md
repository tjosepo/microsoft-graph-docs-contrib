---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

# THE PYTHON SDK IS IN PREVIEW. FOR NON-PRODUCTION USE ONLY

graph_client = GraphServiceClient(request_adapter)

request_body = DeviceLink(
	name = "Backup Link",
)

result = await graph_client.network_access.connectivity.branches.by_branche_id('branchSite-id').device_links.by_device_link_id('deviceLink-id').patch(request_body = request_body)


```