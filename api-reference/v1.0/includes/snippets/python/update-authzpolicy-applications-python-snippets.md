---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

# THE PYTHON SDK IS IN PREVIEW. FOR NON-PRODUCTION USE ONLY

graph_client = GraphServiceClient(request_adapter)

request_body = AuthorizationPolicy(
	default_user_role_permissions = DefaultUserRolePermissions(
		allowed_to_create_apps = False,
	),
)

result = await graph_client.policies.authorization_policy.patch(body = request_body)


```