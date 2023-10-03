---
title: "Enable domain capture in Postman"
updated: 2023-10-01
contextual_links:
  - type: section
    name: "Additional resources"
  - type: subtitle
    name: "Blog posts"
  - type: link
    name: "Introducing Domain Capture: Group Your Organization’s Postman Users into a Single Team"
    url: "https://blog.postman.com/introducing-domain-capture/"
---

> **[Domain verification is available on Postman Enterprise plans. Domain capture is available on Postman Enterprise Ultimate plans.](https://www.postman.com/pricing)**

Now that you've [added and verified a domain](/docs/administration/domain-verification-and-capture/add-and-verify-a-domain/), you can enable domain capture. Domain capture will move all of the existing users who are associated with your verified domain or subdomain to your Enterprise team. Moving forward, any Postman users who sign up for a new account with the relevant domain will be automatically added to your team.

You must be a [Team Admin](/docs/collaborating-in-postman/roles-and-permissions/#team-roles) to enable domain capture in Postman. In addition, your team must have only SAML-based SSO authentication methods enabled to turn on domain capture. Alternative authentication methods such as Postman or Google sign in must be [turned off](/docs/administration/sso/admin-sso/#editing-sso-settings).

## Contents

* [Claim verified accounts](#claim-verified-accounts)

    * [User experience](#user-experience)

    * [Contact support to manage accounts](#contact-support-to-manage-accounts)

* [Domain capture support and FAQs](#domain-capture-support-and-faqs)

## Claim verified accounts

After you've [added and verified](/docs/administration/domain-verification-and-capture/add-and-verify-a-domain/#add-and-verify-a-domain) a domain, you can enable domain capture by navigating to the [domain dashboard](https://go.postman.co/settings/team/domain-capture). To enable domain capture, a Team Admin must create a request with Postman support. Once the request is approved, you can work with Postman support to manage [unclaimed accounts](/docs/administration/domain-verification-and-capture/add-and-verify-a-domain/#view-unclaimed-accounts).

To enable domain capture, do the following:

1. Open Postman and select **Team > Team Settings** in the Postman header. Select **Authentication** in the left sidebar, then select the **Domains** tab.
1. Select **Manage** next to the domain with the **VERIFIED** status you want to enable domain capture for.
1. Select **Request To Claim**. Postman support will then contact Team Admins to explain the effects of enabling domain capture.
1. Once the request is approved, you can [contact Postman support](#contact-support-to-manage-accounts) to manage [unclaimed accounts](/docs/administration/domain-verification-and-capture/add-and-verify-a-domain/#view-unclaimed-accounts).

To view the status of your request to enable domain capture, select **Manage** next to the domain. After you select **Request To Claim**, the request status is changed to **REQUEST SENT**.

![Request to claim sent](https://assets.postman.com/postman-docs/v10/request-to-claim-sent-v10.jpg)

Once the request is approved, a notification will display towards the top of the screen explaining that **Account Capture has been enabled**.

![Domain capture enabled](https://assets.postman.com/postman-docs/v10/domain-capture-enabled-v10.jpg)

> To turn off domain capture, you must [contact Postman support](#contact-support-to-manage-accounts).

### User experience

When domain capture is enabled, new Postman users who sign up for Postman with email addresses associated with your domain or subdomain are automatically added to your team.

Existing Postman users with email addresses associated with the domain or subdomain will only be able to access Postman after joining your team. This applies to existing users who are part of other teams and existing individual users. The next time existing users sign in to Postman, they will get a notification that your team manages their account. Existing users can join the team using this notification.

<img alt="Domain capture join team notification" src="https://assets.postman.com/postman-docs/domain-capture-join-team-9.4.jpg" width="350px"/>

> You won't be able to selectively pick users you'd like to add to your team. Once enabled, the number of unclaimed accounts will reduce as these users sign in and join your team.

Existing users who were on other Postman teams will lose access to all data from their earlier teams, including personal workspaces. No data will be transferred from their earlier teams to their new team. Users won't be able to remain on or join extra Postman teams with their captured accounts.

> To transfer an existing user's collections and environments from their earlier teams to their new team, [contact Postman support](#contact-support-to-manage-accounts).

For more details on the effects of enabling domain capture, see [Domain capture FAQs](/docs/administration/domain-verification-and-capture/domain-capture-support-and-faqs/).

> If users experience any issues when moving to your Postman team, reach out to [Postman support](https://www.postman.com/support/).

### Contact support to manage accounts

Once the request is approved to [enable domain capture](#enable-domain-capture), Team Admins can contact Postman support by navigating to the [domain dashboard](https://go.postman.co/settings/team/domain-capture). Contact Postman support to claim accounts not part of your team, merge teams into your team, and restrict users to only work in your team.

1. Open Postman and select **Team > Team Settings** in the Postman header. Select **Authentication** in the left sidebar, then select the **Domains** tab.

1. Select **Manage** next to the domain with the **VERIFIED** status you want to contact support about.

    > Domain capture must be enabled for the domain you want to contact support about.

1. Select **Contact Support**.

    ![Contact support about managing accounts](https://assets.postman.com/postman-docs/v10/domain-capture-enabled-v10.jpg)

## Domain capture support and FAQs

For more information on the effects of enabling domain capture and how to contact Postman support for assistance, see [Domain capture support and FAQs](/docs/administration/domain-verification-and-capture/domain-capture-support-and-faqs/).
