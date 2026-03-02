# Praktikum Kecerdasan Buatan - Modul 2: Pathfinding

Repositori ini berisi implementasi **Pathfinding** menggunakan **NavMesh (Navigation Mesh)** di Unity. Proyek ini mendemonstrasikan bagaimana AI (Enemy) dapat mencari jalur terpendek untuk mengejar target secara otomatis dan menghindari rintangan (Obstacles).

## 📝 Deskripsi Tugas
Tujuan dari praktikum ini adalah memahami cara kerja komponen NavMesh di Unity, yang meliputi:
1.  **NavMesh Surface**: Pembuatan area yang bisa dilalui oleh agen.
2.  **NavMesh Agent**: Karakter yang memiliki kecerdasan untuk bergerak mencari jalur.
3.  **NavMesh Obstacle**: Objek penghalang yang harus dihindari oleh agen.

## 🛠️ Fitur & Implementasi
- **Enemy Chasing**: Menggunakan script C# untuk menggerakkan agen menuju posisi target secara real-time.
- **Dynamic Movement**: Agen mampu menentukan jalur terbaik meskipun target terus berpindah tempat.
- **Baking NavMesh**: Pengaturan area navigasi pada objek statis di dalam scene.

## 💻 Kode Utama (`enemychasing.cs`)
Implementasi sederhana untuk pergerakan musuh:
```csharp
void Update()
{
    // Mengatur tujuan pergerakan agen ke posisi target setiap frame
    agent.SetDestination(target.position);
}
