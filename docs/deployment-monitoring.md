# Model Deployment and Monitoring Best Practices

Best practices for deploying machine learning models are given below.

## Best Practices

- **Versioning**: Keep a record of all the model versions you have deployed in BigML. This makes it easy to go back to an older version if something goes wrong.
  
- **Performance Monitoring**: : Regularly check how well the model is making predictions by using new data. This helps to spot if the model's accuracy is getting worse over time (called model drift).

- **Logging**: Keep a record of all API requests and the model’s prediction results. This helps in checking what happened (auditing) and fixing any issues (debugging).
  
- **Backup**: Regularly export and back up critical models and datasets.

BigML supports both batch predictions and API-based predictions. Select the appropriate methods based on  needs of your application.
