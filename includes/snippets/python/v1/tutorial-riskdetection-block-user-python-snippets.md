---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

# THE PYTHON SDK IS IN PREVIEW. FOR NON-PRODUCTION USE ONLY

graph_client = GraphServiceClient(request_adapter)

request_body = ConditionalAccessPolicy(
	display_name = "Policy for risky sign-in block access",
	state = ConditionalAccessPolicyState.Enabled,
	conditions = ConditionalAccessConditionSet(
		sign_in_risk_levels = [
			RiskLevel.High,
			RiskLevel.Medium,
		]
		applications = ConditionalAccessApplications(
			include_applications = [
				"All",
			]
		),
		users = ConditionalAccessUsers(
			include_users = [
				"4628e7df-dff3-407c-a08f-75f08c0806dc",
			]
		),
	),
	grant_controls = ConditionalAccessGrantControls(
		operator = "OR",
		built_in_controls = [
			ConditionalAccessGrantControl.Block,
		]
	),
)

result = await graph_client.identity.conditional_access.policies.post(body = request_body)


```