# Menggunakan image Node.js sebagai base image
FROM node:16

# Set working directory di dalam container
WORKDIR /usr/src/app

# Menyalin package.json dan package-lock.json ke dalam container
COPY package.json ./
COPY package-lock.json ./

# Menginstall dependencies
RUN npm install

# Menyalin seluruh kode sumber ke dalam container
COPY . .

# Mengekspos port yang digunakan oleh aplikasi
EXPOSE 8080

# Menjalankan aplikasi
CMD ["node", "src/index.js"]