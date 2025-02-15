#Project Setup Guide

##🚀 Running the Container with Environment Variables
##🐳 Using Docker

##1️⃣ Install the Image

```sh
docker pull dnyaneshwari388/iitm_tds
```

##2️⃣ Run the Container with an .env File
If you have a .env file with environment variables:

```
sh
AIPROXY_TOKEN=your_actual_token
```

Run the container using:

```
sh
docker run --env-file .env -e EXTRA_VAR=value -p 8000:8000 dnyaneshwari388/iitm_tds
```

##3️⃣ Run without .env 
```
sh
docker run  -e AIPROXY_TOKEN=your_actual_token -p 8000:8000 dnyaneshwari388/iitm_tds
```


##🐧 Using Podman

```
sh
podman run -e AIPROXY_TOKEN=your_actual_token -p 8000:8000 dnyaneshwari388/iitm_tds
```
