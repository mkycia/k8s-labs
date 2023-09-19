# LAB-02

```
1. git clone https://github.com/docker/getting-started-app.git

2. cd getting-started-app

3. tee Dockerfile <<EOF
FROM node:18-alpine
WORKDIR /app
COPY . .
RUN yarn install --production
CMD ["node", "src/index.js"]
EXPOSE 3000
EOF

4. docker build -t getting-started:v1 .

5. docker images

```