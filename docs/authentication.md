# Authentication Best Practices

The BigML API uses special codes called API keys to check who is making a request. These keys act like passwords for your machine learning projects. If someone else gets access to your API key, they could use your account,  get access your data,they can  change your models, or even cause extra charges. That is why,it’s very important to keep your API keys private and secure. So,never share them in public places like code files, websites, or emails.

## Best Practices

- You should never expose your secret API key in publicly accessible areas such as client-side code, GitHub repositories, or online forums.
- You should use environment variables or secure vaults to store keys in development and production envirnment
- You should implement multi-factor authentication (MFA) using external systems to secure your BigML account.
- You should only generate keys with permissions necessary for the task.

## Example: Using API Key in HTTP Header

```http
Authorization: Bearer YOUR_BIGML_API_KEY
```

