# Practical Examples Using Secure API Usage

## Example 1: Securely Calling BigML API with Node.js

```javascript
require('dotenv').config();
const fetch = require('node-fetch');

const API_KEY = process.env.BIGML_API_KEY;
const BASE_URL = 'https://bigml.io/andromeda/api/andromeda';

async function getModels() {
  const response = await fetch(`${BASE_URL}/model`, {
    headers: {
      'Authorization': `Bearer ${API_KEY}`,
      'Content-Type': 'application/json'
    }
  });

  if (!response.ok) {
    throw new Error('Failed to fetch models');
  }
  const data = await response.json();
  console.log('Models:', data.objects);
}

getModels().catch(console.error);
```

## Rotating API Keys 

 Step-by-step:

  Generate a new API key via BigML dashboard.

  Update environment secrets in your deployment pipeline.
  
  Redeploy your application using the new key.
  
  Delete or remove the old API key after confirming the new one works.



 