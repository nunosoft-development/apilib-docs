---
title: Adding a Custom Domain to Your Project
description: API-Lib allows you to customize the domain for your project, giving it a personalized touch. This feature is available with the Essentials subscription plan. By following the steps outlined below, you can easily set up a custom domain for your project.
---

## Introduction

API-Lib allows you to customize the domain for your project, giving it a personalized touch. This feature is available with the Essentials subscription plan. By following the steps outlined below, you can easily set up a custom domain for your project.

## Prerequisites

Before proceeding with the custom domain setup, please ensure that you have:

- An active API-Lib account.
- An Essentials subscription plan.
- Access to your project settings.

## Step 1: Access Project Settings

1. Log in to your API-Lib account.
2. Select the desired project for which you want to add a custom domain.
3. Navigate to the **Project Settings** page.


## Step 2: Update Project Custom Domain

1. Within the **Project Settings** page, click on the **Project** tab.
2. Scroll down to the **Project Custom Domain** setting.
3. Click on the **Update** button.

![Update Custom Domain](https://i.nunosoft.net/docs/edit-domain.gif)
[Open GIF](https://i.nunosoft.net/docs/edit-domain.gif)

## Step 3: Enter Your Custom Domain

1. Upon clicking the **Update** button, an input field will appear.
2. Enter your desired custom domain in the provided input field.

## Step 4: Save and Error Handling

1. After entering the custom domain, click on the **Save** button.
2. In case the domain is invalid or not yet set up, an error message will be displayed. The error message might look like this: "Domain is invalid. It needs to contain a TXT DNS entry with the content: 64690718f9c93932a893552e."

## Step 5: Setting up the Domain

To properly set up the domain, you need to add a TXT DNS entry with your project ID to the domain. Follow the steps below, using the example of adding a TXT record for `api-lib.me` on Cloudflare:

1. Log in to your Cloudflare or DNS ptovider account.
2. Select the desired domain (e.g., `api-lib.me`).
3. Navigate to the DNS settings for your domain.
4. Add a new TXT record.
5. In the **Name** or **Host** field, enter `@` or leave it blank to represent the root domain.
6. In the **Value** or **Content** field, enter your project ID. You can find the project ID by following the guide provided [here](https://api-lib.com/guides/finding-project-id).

![Add TXT Record](https://i.nunosoft.net/docs/cloudflare-txt.gif)
[Open GIF](https://i.nunosoft.net/docs/cloudflare-txt.gif)

## Step 6: Verify TXT Record

To ensure the TXT record has been added successfully, you can use a website like [nslookup.io](https://www.nslookup.io/txt-lookup/) to perform a DNS lookup. Enter your domain name and select the TXT record option to check if the TXT record is present and has propagated correctly.

## Step 7: Add Custom Domain to Your API-Lib Project

To complete the setup and avoid any error messages, you need to add the verified custom domain to your API-Lib project. Follow the steps below:

1. Return to the **Project Settings** page in your API-Lib account.
2. Select the desired project for which you added the custom domain.
3. In the **Project Custom Domain** section, click on the **Update** button.
4. Enter your verified custom domain in the input field.
5. Click on the **Save** button to save the changes.


## Step 8: Add A Record for Redirection

To redirect requests to the API-Lib servers, you need to add an A record for the domain. Follow the steps below:

1. Return to your domain's DNS settings on your DNS provider (e.g., Cloudflare).
2. Add a new A record.
3. In the **Name** or **Host** field, enter the desired subdomain or leave it blank to represent the root domain.
4. In the **IPv4 Address** or **Value** field, enter the API-Lib server IP address provided in the project settings. The IP address can be found in parentheses next to your domain.

For example, if the IP address provided in the project settings is `(192.0.2.123)`, you would enter `192.0.2.123` as the IPv4 Address or Value.

![Add A Record](https://example.com/images/add_a_record_cloudflare.png)

Note: The IP address shown in the example above is for demonstration purposes only. Make sure to use the specific IP address provided in your API-Lib project settings.

Once you've added the A record, DNS propagation may take some time. It typically resolves within a few hours, but it can vary depending on your DNS provider. After the propagation is complete, requests to your custom domain will be redirected to the API-Lib servers, enabling seamless access to your API-Lib project.

Congratulations! You have successfully added an A record to your custom domain, completing the setup process for your API-Lib project. If you have any further questions or need assistance, please don't hesitate to reach out to the API-Lib support team.

We hope you enjoy the enhanced branding and control that a custom domain provides for your API-Lib project!