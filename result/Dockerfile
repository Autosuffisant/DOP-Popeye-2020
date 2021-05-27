FROM node:lts-alpine3.12
RUN mkdir views
FROM mhart/alpine-node:12
COPY . .
RUN npm install
ENV PORT=80
EXPOSE 80
CMD ["node", "server.js"]