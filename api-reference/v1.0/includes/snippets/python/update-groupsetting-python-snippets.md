---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

# THE PYTHON SDK IS IN PREVIEW. FOR NON-PRODUCTION USE ONLY

graph_client = GraphServiceClient(request_adapter)

request_body = GroupSetting(
	values = [
		SettingValue(
			name = "AllowToAddGuests",
			value = "true",
		),
	]
)

result = await graph_client.groups.by_group_id('group-id').settings.by_setting_id('groupSetting-id').patch(request_body = request_body)


```