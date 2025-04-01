# Sử dụng Node.js 18 làm base image
FROM node:18

# Đặt thư mục làm việc trong container
WORKDIR /app

# Sao chép file package.json vào container
COPY package.json package-lock.json ./

# Cài đặt dependencies
RUN npm install

# Sao chép toàn bộ source code vào container
COPY . .

# Expose cổng 3000
EXPOSE 3000

# Chạy ứng dụng
CMD ["node", "server.js"]
