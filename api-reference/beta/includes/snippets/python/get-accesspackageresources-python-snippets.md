---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

# THE PYTHON SDK IS IN PREVIEW. FOR NON-PRODUCTION USE ONLY

graph_client = GraphServiceClient(request_adapter)

query_params = AccessPackageResourcesRequestBuilder.AccessPackageResourcesRequestBuilderGetQueryParameters(
		filter = "resourceType eq 'Application'",
		expand = ["accessPackageResourceScopes"],
)

request_configuration = AccessPackageResourcesRequestBuilder.AccessPackageResourcesRequestBuilderGetRequestConfiguration(
query_parameters = query_params,
)

result = await graph_client.identity_governance.entitlement_management.acce_package_catalogs.by_acce_package_catalog_id('accessPackageCatalog-id').acces_package_resources.get(request_configuration = request_configuration)


```