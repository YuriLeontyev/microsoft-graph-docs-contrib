---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

# THE PYTHON SDK IS IN PREVIEW. FOR NON-PRODUCTION USE ONLY

graph_client = GraphServiceClient(request_adapter)

query_params = GroupsRequestBuilder.GroupsRequestBuilderGetQueryParameters(
		search = "\"displayName:OneVideo\" OR \"mail:onevideo\"",
)

request_configuration = GroupsRequestBuilder.GroupsRequestBuilderGetRequestConfiguration(
query_parameters = query_params,
headers = {
			'ConsistencyLevel' : "eventual",
}

)

result = await graph_client.groups.get(request_configuration = request_configuration)


```