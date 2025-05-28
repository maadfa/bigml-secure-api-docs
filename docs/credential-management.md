
---

## 📝 3. `docs/credential-rotation.md` – Credential Management & Rotation

```markdown
# Credential Management and Rotation

Regularly rotating API credentials reduces the risk of compromised keys being abused.

## Recommended Practices

- Establish a key rotation schedule (e.g., every 60–90 days), even if no known issues have occurred.
- Delete old keys promptly after replacement.
- Automate rotation using CI/CD pipelines, secret management tools such as HashiCorp Vault or AWS Secrets Manager, or automation scripts.
- Securely notify your team when rotating keys and provide access through secure channels.

## Example: Testing New Credentials with cURL

```bash
curl -X GET https://bigml.io/andromeda/api/andromeda \
 -H "Authorization: Bearer NEW_API_KEY"
