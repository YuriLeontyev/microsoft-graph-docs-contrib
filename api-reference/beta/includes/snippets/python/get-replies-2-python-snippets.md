---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

# THE PYTHON SDK IS IN PREVIEW. FOR NON-PRODUCTION USE ONLY

graph_client = GraphServiceClient(request_adapter)


result = await graph_client.drives.by_drive_id('drive-id').items.by_item_id('driveItem-id').workbook.comments.by_comment_id('workbookComment-id').replies.get()


```