---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

# THE PYTHON SDK IS IN PREVIEW. FOR NON-PRODUCTION USE ONLY

graph_client = GraphServiceClient(request_adapter)

request_body = BookingBusiness(
	display_name = "Fourth Coffee",
	address = PhysicalAddress(
		post_office_box = "P.O. Box 123",
		street = "4567 Main Street",
		city = "Buffalo",
		state = "NY",
		country_or_region = "USA",
		postal_code = "98052",
	),
	phone = "206-555-0100",
	email = "manager@fourthcoffee.com",
	web_site_url = "https://www.fourthcoffee.com",
	default_currency_iso = "USD",
)

result = await graph_client.booking_businesses.post(body = request_body)


```