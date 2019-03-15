# Golang-based-web

This project is the Golang based backend for media sharing web project. [Media sharing web application](https://github.com/helibu/Media-Sharing-web)

<br> Deployed on http://34.73.107.83/api/v1
## Technology Used
### GCE

### ElasticSearch

### Google ML Engine

### BigTable --> DataFlow --> BigQuery

### GKE


## Supported Endpoint

### "/signup"
For sign up to the web. 

### "/login"
For log in to the web

### "/post"

Make a image/video post to the server. ElasticSearch will store the post info. If the post is a '.jpeg' image post, the ML model on Google ML Engine will predict whether the image is a human face or not.

### "/search"
To search post with a lat, lon and range.


