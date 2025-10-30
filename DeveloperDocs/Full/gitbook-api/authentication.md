---
icon: key
---

# Authentication

<mark style="color:purple;">The GitBook API uses Personal access tokens to authenticate requests.</mark>

<mark style="background-color:green;">You</mark> can <mark style="color:$success;">view</mark> and manage your access tokens in the [Developer settings](https://app.gitbook.com/account/developer) of your GitBook user account.

API requests are authenticated using the [Bearer Auth scheme](https://developer.mozilla.org/en-US/docs/Web/HTTP/Authentication#authentication_schemes). To authenticate a request, provide the token in the `Authorization` header of the request: <mark style="color:blue;">Datacap Token</mark>

```bash
curl -H "Authorization: Bearer <your_access_token>" https://api.gitbook.com/v1/user
```

Access tokens are tied to the GitBook user account for which they were created. **A token provides the same level of access & privileges that its associated GitBook user account would have.**

{% hint style="warning" %}
Please be sure to keep your API access tokens secure! Do not share them in emails, chat messages, client-side code or publicly accessible sites.

If you have accidentally shared an API access token publicly, you can revoke it in the [Developer settings](https://app.gitbook.com/account/developer) of your GitBook user account by clicking the X button beside the token.
{% endhint %}
