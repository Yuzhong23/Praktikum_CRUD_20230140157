Markdown
# Dokumentasi Proyek: User Management System

Proyek ini adalah aplikasi manajemen data pengguna yang mengimplementasikan operasi CRUD (Create, Read, Update, Delete). Dokumentasi ini mencakup hasil pengujian API menggunakan Postman dan tampilan dashboard pada sisi klien.

---

## 🖥️ Tampilan Dashboard
- <img width="1512" height="866" alt="Screenshot 2026-03-03 at 11 39 11" src="https://github.com/user-attachments/assets/86f14db6-d378-4b03-96bb-6edc62cf1c45" />
---

## 🛠️ Dokumentasi Pengujian API (Postman)

Seluruh endpoint diarahkan ke base URL: `http://localhost:8080/api/users`

### 1. Ambil Semua Data (GET)
Mengambil daftar lengkap pengguna yang terdaftar dalam sistem.
- **Method:** `GET`
**Status:** `200 OK`
- **Response:**
```json
{
    "status": "success",
    "data": [
        {
            "age": 0,
            "id": "88343a6f-d318-46d8-9e60-2803494de8c6",
            "name": "Alucard "
        },
        {
            "age": 0,
            "id": "a1c5b371-83dc-4089-a058-58a85c6f8133",
            "name": "Zilong "
        }
    ]
}
2. Tambah Pengguna Baru (POST)
Menambahkan data entitas pengguna baru ke dalam sistem.

Method: POST

Status: 201 Created

Body (JSON):

JSON
{
    "name": "zilong ",
    "age": " 21"
}
Response:

JSON
{
    "status": "success",
    "data": {
        "age": 21,
        "id": "dd34f622-cb93-4507-a27a-7bb7029ae7f8",
        "name": "zilong "
    }
}
3. Perbarui Data Pengguna (PUT)
Mengubah informasi pengguna berdasarkan ID yang spesifik.

Method: PUT

Endpoint: /api/users/01adf8d4-2188-4d7e-a217-ba1778aa403b

Status: 200 OK

Body (JSON):

JSON
{
    "name": "lord",
    "age": " 21"
}
Response:

JSON
{
    "status": "success",
    "data": {
        "age": 21,
        "id": "01adf8d4-2188-4d7e-a217-ba1778aa403b",
        "name": "lord"
    }
}
4. Hapus Data Pengguna (DELETE)
Menghapus data pengguna secara permanen dari database menggunakan ID.

Method: DELETE

Endpoint: /api/users/01adf8d4-2188-4d7e-a217-ba1778aa403b

Status: 200 OK

Response:

JSON
{
    "status": "success delete user with id 01adf8d4-2188-4d7e-a217-ba1778aa403b"
}
