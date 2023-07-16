# text2image-free
![Version badge](https://img.shields.io/badge/version-beta--0.1-green)
![Status badge](https://img.shields.io/badge/status-offline-red)

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

### GET https://api.sitius.tech/gen

#### Simply returns some preferred models.
