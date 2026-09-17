# MBA Workshop, September 2026

### Locations
- London, 23rd September 2026
- Dubai, 30th September 2026

### Pre-workshop instructions
- Ensure admin access to your Business Manager.
- Follow [the instructions](https://developers.facebook.com/documentation/meta-business-agent/get-started#step-1-set-up-meta-business-agent-in-whatsapp-manager) to accept ToS.
- Ensure Meta Business Agent Payment Method is configured in Bulling Hub.
- Prepare WhatsApp Business Account and a phone_number onboarded to WhatsApp Cloud API. Ensure messaging works.
- Prepare Meta Product Catalog and connect it to WhatsApp Business Account if you want MBA uses your product catalog.
- Prepare BISU token with scopes - **whatsapp_business_management** and **whatsapp_business_messaging**.

### Files
- MBA-Workshop.postman_collection.json - Postman collection of API calls
- MBA-Workshop.postman_environment.json - environment variables for Postman

### Developers documentation
- https://developers.facebook.com/documentation/meta-business-agent

### Workshop instructions
#### 1. Import collections into Postman.
#### 2. Select the "MBA Workshop — env (Store API)" environment.
#### 3. Fill in variables:

| Variable	| Value |
| --- | --- |
| `ENTITY_ID` |	Your WhatsApp Business Phone Number ID |
| `MBA_ACCESS_TOKEN` |	A token with the whatsapp_business_messaging permission |
| `CONSUMER_PHONE` |	Your own test number in E.164, e.g. +5511999998888 |
| `SUPPORT_PHONE` |	The number the agent points at when it hands off, digits only |

#### 4. Run API calls one-by-one.

Note: `AGENT_ID` and `CONNECTOR_ID` variables are captured automatically, nothing to copy-paste between requests.

#### 5. Mock tools - E-commerce Simulator

| Variable	| Value
| --- | --- |
| `SHOP_API_KEY` | a API key for DemoStore will be provided at the workshop |
| `SHOP_API` | API endpoint for DemoStore  will be provided at the workshop |

#### 6. Workshop outcome

The fully working agent that answers customers questions from live product catalog data, renders results as interactive messages.
The agent is unable take orders — cart, checkout and payments are out of scope.

Thank you!



