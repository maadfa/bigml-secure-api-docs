# Authentication Best Practices

BigML API uses API keys to authenticate requests. It is essential to protect your API keys to prevent unauthorized access.

## Best Practices

- Never expose your secret API key in publicly accessible areas such as client-side code, GitHub repositories, or online forums.
- Use environment variables or secure vaults to store keys in development and production envirnment
- Implement multi-factor authentication (MFA) using external systems to secure your BigML account.
-  Only generate keys with permissions necessary for the task.

## Example: Using API Key in HTTP Header

```http
Authorization: Bearer YOUR_BIGML_API_KEY
```

