---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

# THE PYTHON SDK IS IN PREVIEW. FOR NON-PRODUCTION USE ONLY

graph_client = GraphServiceClient(request_adapter)

request_body = TeamworkTag(
	display_name = "Finance",
)

result = await graph_client.teams.by_team_id('team-id').tags.by_tag_id('teamworkTag-id').patch(request_body = request_body)


```