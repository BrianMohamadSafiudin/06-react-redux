### Nama : Brian Mohamad Safiudin
### NIM : 2141720133
### Kelas : TI-3A
---

# Praktikum 1: Instalasi Redux dan bootstrap

#### Edit file pages/index.tsx menjadi seperti ini.

```tsx
export default function Home() {
  return (      
    <div className="container">
      <div className="row">
        <div className="col-12">
          <button type="button"
                  className="btn btn-primary"
                  data-bs-toggle="modal"
                  data-bs-target="#exampleModal">
                  Coba Model Bootstrap
          </button>
        </div>
      </div>
      <div  className="modal fade"
            id="exampleModal"
            tabIndex="-1"
            aria-labelledby="exampleModalLabel"
            aria-hidden="true">
        <div className="modal-dialog">
          <div className="modal-content">
            <div className="modal-header">
              <h5 className="modal-title text-black" id="exampleModalLabel"> yay... </h5>
              <button
                type="button"
                className="btn-close"
                data-bs-dismiss="modal"
                aria-label="Close"></button>
            </div>
            <div className="modal-body text-black">
              <h2>Halo semua, kita sedang menggunakan bootstrap di Next.js</h2>
            </div>
          </div>
        </div>
      </div>
    </div>
  );
}
```

#### Coba kita jalankan project next.js kita, dan laporkan apa yang terjadi?

![GIF P1](assets-report/praktikum1.gif)

- muncul tampilan dengan button "Coba Model Bootstrap", lalu muncul tulisan "yay... dan Halo semua, kita sedang menggunakan bootstrap di Next.js".

---

# Praktikum 2: Contoh Login dengan Redux

## Soal 1
#### Coba akses http://localhost:3000/login, dan klik tombol login. Kemudian lakukan refresh page berkali-kali (jika perlu restart npm run dev nya). Simpulkan apa yang terjadi ?

![GIF P2](assets-report/praktikum2a.gif)

- Setelah melakukan refresh page berkali-kali, maka akan muncul pesan "Yay, berhasil login !!!" dan apabila logout maka akan muncul pesan "Anda telah logout". Hal ini terjadi karena kita menggunakan Redux untuk menyimpan data login dan logout sehingga data tersebut tidak akan hilang ketika kita melakukan refresh page atau restart npm run dev nya

## Soal 2
#### Baris 25 dan 30 terdapat method parse(), apa yang terjadi jika kita tidak menggunakan method tersebut?

![GIF P2](assets-report/praktikum2b.gif)

- Jika kita tidak menggunakan method parse(), maka akan muncul tampilan mentahan dari div karena parse digunakan untuk mengubah string menjadi objek.

---

# Praktikum 3: Membuat Aplikasi Counter Sederhana

#### kita jalankan di browser dengan url localhost:3000/counter, dan amati apa yang terjadi?

![GIF P3](assets-report/praktikum3.gif)

- Muncul tampilan counter sederhana dengan button tambah dan kurang, dan angka counter yang bertambah atau berkurang sesuai dengan button yang ditekan.

---