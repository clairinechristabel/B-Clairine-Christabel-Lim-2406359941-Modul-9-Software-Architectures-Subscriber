# Understanding Subscriber and Message Broker

## a. What is AMQP?
**AMQP (Advanced Message Queuing Protocol)** adalah protokol standar terbuka pada *application layer* yang digunakan untuk komunikasi *middleware* berorientasi pesan (*Message-Oriented Middleware*). Protokol ini memungkinkan berbagai aplikasi atau sistem (yang mungkin ditulis dengan bahasa pemrograman berbeda atau berjalan di *platform* yang berbeda) untuk saling berkomunikasi dan bertukar pesan secara aman, andal, dan terstandarisasi. RabbitMQ adalah salah satu perangkat lunak *message broker* populer yang mengimplementasikan protokol AMQP.

## b. What does it mean? `guest:guest@localhost:5672`
Format URL `guest:guest@localhost:5672` adalah *connection string* standar yang digunakan untuk melakukan koneksi ke layanan *message broker* (seperti RabbitMQ) menggunakan protokol AMQP. Berikut adalah rinciannya:

- **`guest` (pertama)**: Merupakan *username* (nama pengguna) default untuk autentikasi ke dalam server RabbitMQ.
- **`guest` (kedua)**: Merupakan *password* (kata sandi) default yang berpasangan dengan username tersebut.
- **`localhost:5672`**: Menunjukkan lokasi server dan port jaringan.
  - **`localhost`**: Merupakan alamat *host* tempat server *message broker* berjalan. `localhost` berarti server tersebut berjalan di komputer lokal kita sendiri (IP `127.0.0.1`).
  - **`5672`**: Merupakan *port default* yang digunakan oleh protokol AMQP (khususnya RabbitMQ) untuk mendengarkan dan menerima koneksi masuk dari *publisher* maupun *subscriber*.
