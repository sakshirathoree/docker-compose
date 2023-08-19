FROM node

WORKDIR /app

COPY package*.json .

RUN npm install

# Add node_modules to the PATH environment variable
ENV PATH /app/node_modules/.bin:$PATH

COPY . .

EXPOSE 80

ENV MONGODB_USERNAME=root
ENV MONGODB_PASSWORD=secret

CMD ["npm", "start"]