FROM node:23-alpine
WORKDIR /app
COPY package.json .
RUN npm install --only=prod
COPY . .
EXPOSE 4001
USER node
CMD ["npm", "run", "listen"]