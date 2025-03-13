FROM node:20-bullseye

WORKDIR /app

COPY app/package.json app/package-lock.json app/tsconfig.json ./

RUN npm install

COPY app ./

RUN npm run build

EXPOSE 3000

CMD ["npm", "run", "start:dev"]
