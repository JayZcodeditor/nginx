# ใช้ Node.js base image
FROM node:14

# ตั้งค่าทำงานใน /usr/src/app
WORKDIR /usr/src/app

# คัดลอกไฟล์ package.json และ package-lock.json (ถ้ามี)
COPY package*.json ./

# ติดตั้ง dependencies
RUN npm install

# คัดลอกไฟล์โค้ดทั้งหมดไปยัง container
COPY . .

# เปิดพอร์ต 8000
EXPOSE 3000

# คำสั่งเริ่มต้น
CMD ["npm", "start"]
