# Lab 2 - Employee CRUD (Flask)

Tugas Lab Pemrograman: menambahkan tombol **Update** dan **Delete** data employee.

## Fitur
- Tambah employee (form)
- **Edit/Update** employee (tombol "Edit" di setiap baris)
- **Hapus/Delete** employee (tombol "Hapus" dengan konfirmasi)
- API JSON: `GET /employees`, `GET /employees/<id>`

## Route baru
| Method | URL | Fungsi |
|---|---|---|
| GET | `/employees/<id>/edit` | Tampilkan form edit |
| POST | `/employees/<id>/edit` | Simpan perubahan data |
| POST | `/employees/<id>/delete` | Hapus data employee |

## Cara menjalankan
```bash
python -m venv .venv
source .venv/bin/activate      # Windows: .venv\Scripts\activate
pip install -r requirements.txt
python app.py
```
Buka http://127.0.0.1:5000/employees/new
