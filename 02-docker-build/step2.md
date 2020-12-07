# ສ້າງ Docker Image

ສ້າງໄຟລ໌ Dockerfile

```dockerfile
FROM node:12
WORKDIR /app
COPY package.json .
RUN npm install
COPY  . .
CMD ["npm", "run", "start"]
```

ສ້າງ Docker Image
`docker build -t nodeapp .`

ເບິ່ງ Docker Image ທີ່ສ້າງ
`docker images`

ຣັນ Container ຈາກ Image ທີ່ສ້າງ
`docker run --name nodeapp -p 8080:8080 --rm nodeapp`
