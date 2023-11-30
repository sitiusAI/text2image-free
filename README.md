# NOTICE
Due to performence issues we are announcing the closure of this api.
We will be creating a new version using google cloud soon.
During this period the api will remain running but without any updates. this includes security and maintenence updates. No matter the case we will not provide support on this API.

[potential alternative](https://github.com/sitiusAI/text2image-free/issues/7)


# text2image-free
![Version badge](https://img.shields.io/badge/version-beta--0.1-blue)
![Status badge](https://img.shields.io/badge/status-online-green)

# URL 
## https://api.sitius.tech

# Usage
## Swagger generated documentation
##### https://api.sitius.tech/docs

# Detailed usage

## Endpoints

### POST https://api.sitius.tech/gen

#### example json

```
{
  "prompt": "cute dog",
  "negative": "bad anatomy",
  "model": "runwayml/stable-diffusion-v1-5"
}
```

Here you can use any text2image pipeline model available to huggingface.
Simply set the model field with the huggingface model id field (it should look like **username/model**)

response will contain an url to the image

### GET https://api.sitius.tech/models

#### Simply returns some preferred models.

## Example by language

### Python

```python
import requests

API_URL = "https://api.sitius.tech"

def query(payload):
	response = requests.post(API_URL, json=payload)
	return response.content
image_bytes = query({
  "prompt": "cute dog",
  "negative": "bad anatomy",
  "model": "runwayml/stable-diffusion-v1-5"
})
```

### Javascript

```js
async function query(data) {
	const response = await fetch(
		"https://api.sitius.tech",
		{
			method: "POST",
			body: JSON.stringify(data),
		}
	);
	const result = await response.blob();
	return result;
}
query({"prompt": "cute dog", "negative": "bad anatomy", "model": "runwayml/stable-diffusion-v1-5"}).then((response) => {
	// Use image
});
```

# License

Use this however you like. Give it a star and if you want credits in your app
