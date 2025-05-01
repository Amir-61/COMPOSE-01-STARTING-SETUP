FROM node

WORKDIR /app

COPY package.json .

RUN npm install
# # ⬇️ Add this if nodemon is a devDependency:
# RUN npm install -g nodemon

COPY . .

EXPOSE 80

ENV MONGODB_USERNAME=root
ENV MONGODB_PASSWORD=secret

CMD ["npm", "start"]