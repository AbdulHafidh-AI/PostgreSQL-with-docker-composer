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

<ul>
  <li>"docker composer" adalah perintah untuk menjalankan file docker-compose.yml, yang berisi definisi services, image, volume, network, dan konfigurasi lainya. </li>
  <li>Perintah "up" digunakan untuk memulai dan menjalankan semua layanan yang didefinisikan di dalam docker-compose.yml</li>
  <li>Tanpa "-d", proses akan tetap terlihat di terminal, dan tetap akan menampilkan log secara real-time. </li>
</ul>

### 2. Access the database 
<pre></code> docker exec -it postgres_container psql -U myuser -d mydatabase </code> </pre>

<ul>
  <li> "postgres_container" merupakan nama container yang digunakan di repositori ini </li>
  <li> "-U <username>": Username PostgreSQL (contoh: myuser). </li>
  <li> "-d <database_name>": Nama database yang ingin diakses (contoh: mydatabase). </li>
</ul>

### 3. Exit database
<pre></code> Exit </code> </pre>

### 4. Switch off PostgreSQL image
<pre><code> docker composer down </code></pre>
<p>"docker compose down" akan menghentikan container dan menghapus network serta volume yang dibuat oleh docker-compose</p>





