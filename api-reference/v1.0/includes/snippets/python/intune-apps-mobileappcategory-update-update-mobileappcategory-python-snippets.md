---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

# THE PYTHON SDK IS IN PREVIEW. FOR NON-PRODUCTION USE ONLY

graph_client = GraphServiceClient(request_adapter)

request_body = MobileAppCategory(
	odata_type = "#microsoft.graph.mobileAppCategory",
	display_name = "Display Name value",
)

result = await graph_client.device_app_management.mobile_app_categories.by_mobile_app_categorie_id('mobileAppCategory-id').patch(request_body = request_body)


```