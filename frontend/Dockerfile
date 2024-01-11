FROM node:18
WORKDIR /app

COPY package.json package.json
COPY package-lock.json package-lock.json

COPY . .
RUN npm run build

CMD ["npx", "-y", "http-server", "-p", "8000", "/app/build"]