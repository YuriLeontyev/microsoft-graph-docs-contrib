---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

# THE PYTHON SDK IS IN PREVIEW. FOR NON-PRODUCTION USE ONLY

graph_client = GraphServiceClient(request_adapter)

request_body = EvaluateRemovalPostRequestBody(
	content_info = ContentInfo(
		odata_type = "#microsoft.graph.security.contentInfo",
		identifier = None,
		state = ContentState.Rest,
		metadata = [
			KeyValuePair(
				name = "MSIP_Label_836ff34f-b604-4a62-a68c-d6be4205d569_Enabled",
				value = "True",
			),
			KeyValuePair(
				name = "MSIP_Label_836ff34f-b604-4a62-a68c-d6be4205d569_Method",
				value = "Standard",
			),
			KeyValuePair(
				name = "MSIP_Label_836ff34f-b604-4a62-a68c-d6be4205d569_SetDate",
				value = "1/1/0001 12:00:00 AM",
			),
			KeyValuePair(
				odata_type = "#microsoft.graph.security.keyValuePair",
				name = "MSIP_Label_836ff34f-b604-4a62-a68c-d6be4205d569_SiteId",
				value = "cfa4cf1d-a337-4481-aa99-19d8f3d63f7c",
			),
			KeyValuePair(
				odata_type = "#microsoft.graph.security.keyValuePair",
				name = "MSIP_Label_836ff34f-b604-4a62-a68c-d6be4205d569_Name",
				value = "LabelScopedToBob_Tests",
			),
			KeyValuePair(
				odata_type = "#microsoft.graph.security.keyValuePair",
				name = "MSIP_Label_836ff34f-b604-4a62-a68c-d6be4205d569_ContentBits",
				value = "0",
			),
			KeyValuePair(
				odata_type = "#microsoft.graph.security.keyValuePair",
				name = "MSIP_Label_836ff34f-b604-4a62-a68c-d6be4205d569_ActionId",
				value = "00000000-0000-0000-0000-000000000000",
			),
		]
	),
	downgrade_justification = DowngradeJustification(
		justification_message = "The information has been declassified.",
		is_downgrade_justified = True,
	),
)

request_configuration = EvaluateRemovalRequestBuilder.EvaluateRemovalRequestBuilderPostRequestConfiguration(
headers = {
		'User-Agent' : "ContosoLOBApp/1.0",
}

)

result = await graph_client.users.by_user_id('user-id').security.information_protection.sensitivity_labels.microsoft_graph_security_evaluate_removal.post(body = request_body, request_configuration = request_configuration)


```