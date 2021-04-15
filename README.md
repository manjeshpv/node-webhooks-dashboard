# node-webhooks-dashboard
Dashboard for Developers - https://github.com/roccomuso/node-webhooks

Support one directional - async communication

## Phase 1
### Features
- Logging(without compromising webhook delivery performance)
  - runs as a third party service
    - Logging grade mongodb configs used and separate server for mongodb and nodejs runtime so logging should not affect main application performance
  - with Mongodb
  - [Metabase](https://www.metabase.com/) for reporting & Queries
- Retries from UI for developers
  - Get Curl requests
  - Not bulk retries

### Use cases
- Sending Notifications(Emails, SMS)
- Sideload or keep integrations separate from core login implementations
  - on signup - create employeee account in SalesCRM

## Phase 2 - Integrating with Storage Adapters (SQS, RabbitMQ)
inspired by https://github.com/jstemmer/rehook
- Webhooks from Payment gateways

## Architecture
- https://hookdeck.io/
