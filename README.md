# tugas-monolitg-dan-microservice
## 🚀 Cara Menjalankan Aplikasi

### 1. Prasyarat
Pastikan Python 3 dan pustaka `Flask` serta `requests` sudah terpasang:
```bash
pip install flask requests
2. Menjalankan Versi Monolith
Masuk ke folder Monolith:
cd "Bagian 1: Monolith"
Jalankan aplikasi:
python3 monolith_app.py
Uji di terminal baru:

Cek buku: curl http://localhost:5000/books

Buat pesanan: curl -X POST -H "Content-Type: application/json" -d '{"book_id": 1}' http://localhost:5000/orders

3. Menjalankan Versi Microservices
Jalankan Book Service (Terminal 1):
cd "Bagian 2: Microservices"
python3 book_service.py
Jalankan Order Service (Terminal 2):
cd "Bagian 2: Microservices"
python3 order_service.py
cd "Bagian 2: Microservices"
python3 order_service.py
Pengujian (Terminal 3):

Cek buku: curl http://localhost:5001/books

Buat pesanan: curl -X POST -H "Content-Type: application/json" -d '{"book_id": 1}' http://localhost:5002/orders
