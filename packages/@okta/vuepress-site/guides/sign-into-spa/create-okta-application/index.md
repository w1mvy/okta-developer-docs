---
title: Create an Okta Application
---

Before your code can redirect to Okta to sign a user in, you need to create an Okta Application that represents your single-page application.

First, sign in to the Okta Developer Console:

<a href="https://login.okta.com/" target="_blank" class="Button--blue">Go to Console</a>

Select **Applications**, then **Add Application**. Pick **Single-Page App (SPA)** as the platform. Enter a name for your application (or leave the default value).

Add the **Base URI** of your application that you use for local development, such as `http://localhost:8080`. Also, add any base URIs where your application runs in production, such as `https://app.example.com`.

Next, enter values for the **Login redirect URI**. This is the callback route you created in the [previous step](/guides/sign-into-spa/-/define-callback). You should add values for local development (such as `http://localhost:8080/implicit/callback`) and production (such as `https://app.example.com/implicit/callback`).

Finally, click **Done** to finish creating the Okta Application. You'll need to copy some values into your application later, so leave the Developer Console tab open.

<NextSectionLink/>