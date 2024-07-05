# Gunakan image dasar Python
FROM python:3.9-slim

# Tentukan direktori kerja di dalam container
WORKDIR /app

# Salin file requirements.txt ke direktori kerja
COPY requirements.txt .

# Instal dependensi Python
RUN pip install -r requirements.txt

# Salin seluruh isi direktori proyek ke dalam direktori kerja
COPY . .

# Tentukan port yang akan di-expose
EXPOSE 5000

# Tentukan perintah untuk menjalankan aplikasi
CMD ["python", "app.py"]
