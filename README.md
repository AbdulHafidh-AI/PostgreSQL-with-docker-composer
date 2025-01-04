# PostgreSQL dengan Docker Compose

Panduan ini menjelaskan langkah-langkah menjalankan PostgreSQL menggunakan Docker Compose.

## Prasyarat
Pastikan Anda sudah menginstal:
- [Docker](https://www.docker.com/products/docker-desktop/)
- [Docker Compose](https://docs.docker.com/compose/)

---

## Langkah-langkah

### 1. Menjalankan PostgreSQL menggunakan Docker Compose
Jalankan perintah berikut untuk memulai layanan PostgreSQL:

<pre><code> docker composer up -d </code> </pre>

### 2. Access the database 
<pre></code> docker exec -it postgres_container psql -U myuser -d mydatabase </code> </pre>

### 3. Exit database
<pre></code> Exit </code> </pre>

### 4. Switch off PostgreSQL image
<pre><code> docker composer down </code></pre>





