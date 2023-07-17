# text2image-free
![Version badge](https://img.shields.io/badge/version-beta--0.1-blue)
![Status badge](https://img.shields.io/badge/status-online-green)

# URL 
## https://api.sitius.tech

# Usage
## Swagger generated documentation
##### https://api.sitius.tech/docs

## Detailed usage

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
