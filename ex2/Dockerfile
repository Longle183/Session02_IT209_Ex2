# 1. Base Image: Su dung Node.js 18 tren nen Alpine Linux nhe
FROM node:18-alpine

# 2. Thu muc lam viec ben trong container
WORKDIR /app

# 3. Thiet lap bien moi truong PORT
ENV PORT=3000

# 4. Sao chep package.json truoc de tan dung Docker cache
COPY package*.json ./

# 5. Cai dat cac dependencies
RUN npm install

# 6. Sao chep toan bo ma nguon con lai vao container
COPY . .

# 7. Khai bao cong container lang nghe
EXPOSE 3000

# 8. Lenh khoi chay ung dung o dang exec form
CMD ["node", "server.js"]
