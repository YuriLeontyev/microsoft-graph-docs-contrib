---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

# THE PYTHON SDK IS IN PREVIEW. FOR NON-PRODUCTION USE ONLY

graph_client = GraphServiceClient(request_adapter)

query_params = DeltaRequestBuilder.DeltaRequestBuilderGetQueryParameters(
		start_date_time = "{start_datetime}",
		end_date_time = "{end_datetime}",
)

request_configuration = DeltaRequestBuilder.DeltaRequestBuilderGetRequestConfiguration(
query_parameters = query_params,
headers = {
			'Prefer' : "odata.maxpagesize=2",
}

)

result = await graph_client.me.calendar_view.delta.get(request_configuration = request_configuration)


```