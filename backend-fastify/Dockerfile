FROM node:18
WORKDIR /app
COPY package*.json ./
RUN npm install
RUN npm install mongodb
COPY . .
EXPOSE 8000
CMD ["npm", "run", "dev", "--host", "0.0.0.0", "--port", "8000"]
RUN npm run db:seeder
