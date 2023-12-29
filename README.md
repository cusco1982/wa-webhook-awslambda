# whatsApp Webhook on AWS Lambda

This template demonstrates how to develop and deploy a simple Node Express Webhook Listener with AWS Lambda using the Serverless Framerwork.

### Anatomy of the template

This template configures a single function, api, which is responsible for handling all incoming requests thanks to the httpApi event. To learn more about httpApi event configuration options, please refer to [httpApi event docs](https://www.serverless.com/framework/docs/providers/aws/events/http-api/). As the event is configured in a way to accept all incoming requests, express framework is responsible for routing and handling requests internally. Implementation takes advantage of serverless-http package, which allows you to wrap existing express applications. To learn more about serverless-http, please refer to corresponding [GitHub repository](https://github.com/dougmoscrop/serverless-http).