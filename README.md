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
#### 1. Import both files into Postman.
#### 2. Select the MBA Workshop — ElecStore environment.
#### 3. Fill in variables:

| Variable	| Value |
| --- | --- |
| `ENTITY_ID` |	Your WhatsApp Business Phone Number ID |
| `MBA_ACCESS_TOKEN` |	A token with the whatsapp_business_messaging permission |
| `CONSUMER_PHONE` |	Your own test number in E.164, e.g. +5511999998888 |
| `SUPPORT_PHONE` |	The number the agent points at when it hands off, digits only |

#### 4. Run API call from 01.xxx to 22.xxx one-by-one:

Onboarding → Settings → Business info → FAQs → Behaviour skills → Connector and Tools → Connector skills → Allowlist → Rollout

Note: `AGENT_ID` and `CONNECTOR_ID` variables are captured automatically, nothing to copy-paste between requests.

#### 5. Mock tools - E-commerce Simulator

| Variable	| Value |
| --- | --- |
| `SHOP_API_KEY` | a sandbox key for a shared demo tenant |
| `SHOP_API` | points at a public ecommerce simulator, mock_ecommerce_api |

#### 6. Workshop outcome

The agent that answers "what do you sell?", "how much is it?", "do you have it in black?" and "is it in stock?" from live catalogue data, over WhatsApp — rendering the results as a carousel with tappable buttons rather than a wall of text. It deliberately cannot take an order — cart, checkout and payment are out of scope, and the skills tell it to hand off for anything it has no tool for. Ask it to buy something and watch it pass you to a human rather than invent a checkout. That is the agent working, not failing.

Thank you!



