---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

# THE PYTHON SDK IS IN PREVIEW. FOR NON-PRODUCTION USE ONLY

graph_client = GraphServiceClient(request_adapter)

request_body = ReviewSet(
	display_name = "My Reviewset 3",
)

result = await graph_client.compliance.ediscovery.cases.by_case_id('case-id').review_sets.post(body = request_body)


```