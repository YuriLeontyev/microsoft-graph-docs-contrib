---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

# THE PYTHON SDK IS IN PREVIEW. FOR NON-PRODUCTION USE ONLY

graph_client = GraphServiceClient(request_adapter)

query_params = ServiceHealthRequestBuilder.ServiceHealthRequestBuilderGetQueryParameters(
		expand = ["issues"],
)

request_configuration = ServiceHealthRequestBuilder.ServiceHealthRequestBuilderGetRequestConfiguration(
query_parameters = query_params,
)

result = await graph_client.admin.service_announcement.health_overviews.by_health_overview_id('serviceHealth-id').get(request_configuration = request_configuration)


```