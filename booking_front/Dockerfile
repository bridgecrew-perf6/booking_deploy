FROM node:16.15-alpine
WORKDIR /app
COPY package.json /app/package.json
COPY . .
RUN npm install
EXPOSE 3000
CMD ["npm", "run", "build"]
CMD ["npm", "run", "start"]