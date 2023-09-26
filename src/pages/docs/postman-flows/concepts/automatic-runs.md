---
title: "Automatic runs"
updated: 2023-08-15
---

You can deploy a Flow to the cloud. The Flow can then be run each time it receives a webhook from another service. This enables a Flow to be run automatically in the cloud.

## Contents

* [Basic concepts of Postman Flows and webhooks](#basic-concepts-of-postman-flows-and-webhooks)
* [Testing locally](#testing-locally)
* [Deploy your Flow](#deploy-your-flow)
* [Trigger the webhook](#trigger-the-webhook)

### Basic concepts of Postman Flows and webhooks

Webhooks are a way for one system to tell another system that some information has changed. It works similarly to push notifications on a phone. Instead of constantly checking your email app to see if there's any new mail, the email app sends a notification you that a new email has been received. Many services today with APIs also offer webhooks as a way to communicate between their system and yours.

When a Flow is deployed to the cloud, the Flow can be run each time it receives a webhook event from another service. This is useful because the Flow can be run automatically and doesn't need your computer to be on, since these Flows run on Postman's cloud.

### Testing locally

Every Flow begins with the **Start** block. When you want to create a Flow to run on the cloud, you'll want to test it locally. You can enter information into the **Start** block by selecting the **Start** block then selecting the gear icon <img alt="Gear icon" src="https://assets.postman.com/postman-docs/icon-settings-v9.jpg#icon" width="16px"> in the right sidebar. This information can either be in text or JSON format. Typically, you'll want to put an example of what an actual webhook will be from the API you're working with. Many APIs include a sample of what their webhook information will look like, but if the API you're working with doesn't you can make one yourself by following the steps in the [Trigger the webhook](#trigger-the-webhook) step.

![Testing Locally](https://assets.postman.com/postman-docs/v10/running-flows-on-the-cloud-test-data-v10-1.gif)

### Deploy your Flow

Selecting **Deploy** will take your local Flow and upload it to Postman's cloud. Selecting the **Runs** section of the right pane will show the time and date it was last deployed and the **Webhook Events** sections will list every webhook sent to the deployed Flow.

In the **Runs** section, select **View Deployed** to observe the Flow running in the cloud. Select **View Live Logs** in the bottom middle of the page to see the live information flowing into your Flow. Selecting **Back to Editor** will take you back to your local Flow where you can make changes and then deploy again when you're finished.

> **Important**
>
> Every time you deploy, it saves your collections and environments. If you make any changes to these, you will need to deploy again.

<img alt="Deploy to cloud" src="https://assets.postman.com/postman-labs-docs/concepts/updated-deploy-a-flow.gif" fetchpriority="low" loading="lazy" />

### Trigger the webhook

Often when working with webhooks, there will be another service that will send the webhook to the Flow you deployed. The **Webhook URL** shown in the right panel is the URL that you can provide the other system or service with that tells it where to send notifications to. Once that's set up, you can view the live logs and see what the notification from the other service looks like to use as your test data. Flows can also be manually run by making a POST request to the **Webhook URL**.

![Trigger the Endpoint](https://assets.postman.com/postman-labs-docs/concepts/updated-triggering-a-webhook.gif)
