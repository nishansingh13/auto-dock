FROM node:18

WORKDIR /app

# Install serve to host static files
RUN npm install -g serve

COPY package*.json ./

RUN npm install

COPY . .

EXPOSE 3000

CMD ["serve", "-s", "public", "-l", "3000"]
