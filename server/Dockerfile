# FROM mhart/alpine-node

# WORKDIR /src

# # Install app dependencies
# COPY package.json .
# # For npm@5 or later, copy package-lock.json as well
# # COPY package.json package-lock.json .

# RUN npm i

# # Bundle app source
# COPY . .

# ENV NODE_ENV=production

# EXPOSE 3001

# CMD [ "npm", "start" ]

FROM node:8.2.0-alpine
RUN mkdir -p /usr/src/app
COPY ./app/* /usr/src/app/
WORKDIR /usr/src/app
RUN npm i
CMD ["npm", "start"]