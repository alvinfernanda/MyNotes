# My Notes

## Introduction
My Notes adalah aplikasi Android sederhana untuk membuat, mengedit, dan menghapus catatan. Aplikasi ini menggunakan penyimpanan lokal dengan Room sebagai basis data untuk menyimpan catatan dan menggunakan arsitektur MVVM.

## Features
- Tambah Catatan: Pengguna dapat membuat catatan baru dengan judul dan deskripsi.
- Edit Catatan: Pengguna dapat mengedit catatan yang sudah ada.
- Hapus Catatan: Pengguna dapat menghapus catatan.
- Tampilkan Daftar Catatan: Semua catatan yang disimpan secara lokal ditampilkan dalam daftar.

## Project Structure
```bash
com.example.localnotesapplication
│
├── data
│   ├── Note.java                # Entity kelas untuk catatan
│   ├── NoteDao.java             # Data Access Object untuk operasi database
│   └── NoteDatabase.java        # Room Database untuk catatan
│
├── repository
│   └── NoteRepository.java      # Repository untuk mengelola data dari berbagai sumber
│
├── ui
│   ├── NoteAdapter.java         # Adapter untuk RecyclerView
│   ├── NoteViewModel.java       # ViewModel untuk mengelola UI terkait data catatan
│   └── AddEditNoteActivity.java # Activity untuk menambah/mengedit catatan
│
├── MainActivity.java            # Activity utama yang menampilkan daftar catatan
├── AndroidManifest.xml          # Deklarasi komponen aplikasi
└── res
    └── layout
        ├── activity_main.xml    # Layout untuk MainActivity
        ├── activity_add_edit_note.xml # Layout untuk AddEditNoteActivity
        └── note_item.xml        # Layout untuk item catatan di RecyclerView
```
