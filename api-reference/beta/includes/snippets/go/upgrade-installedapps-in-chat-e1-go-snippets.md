---
description: "Automatically generated file. DO NOT MODIFY"
---

```go


import (
	  "context"
	  msgraphsdk "github.com/microsoftgraph/msgraph-beta-sdk-go"
	  //other-imports
)

graphClient := msgraphsdk.NewGraphServiceClientWithCredentials(cred, scopes)



graphClient.Chats().ByChatId("chat-id").InstalledApps().ByTeamsAppInstallationId("teamsAppInstallation-id").Upgrade().Post(context.Background(), nil)


```