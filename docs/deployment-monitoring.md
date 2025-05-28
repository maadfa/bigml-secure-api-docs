# Model Deployment and Monitoring Best Practices

Best practices for deploying machine learning models are given below.

## Best Practices

- **Versioning**: Keep track of all deployed model versions in BigML to enable easy rollback if necessary.
- **Performance Monitoring**: Continuously evaluate model predictions by using  fresh data to detect model drift.
- **Logging**: Log all API requests and prediction outputs for auditing and debugging purposes.
- **Backup**: Regularly export and back up critical models and datasets.

BigML supports both batch predictions and API-based predictions. Select the appropriate methods based on  needs of your application.
