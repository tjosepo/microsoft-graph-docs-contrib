---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

# THE PYTHON SDK IS IN PREVIEW. FOR NON-PRODUCTION USE ONLY

graph_client = GraphServiceClient(request_adapter)

request_body = OutlookTaskFolder(
	name = "Volunteer",
)

result = await graph_client.me.outlook.task_folders.post(request_body = request_body)


```