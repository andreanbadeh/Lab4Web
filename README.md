# Praktikum Pemrograman Web 1
Nama : ANDREAN PUTRA ARYA

NIM : 312410341

KELAS : TI.24.A.4

# Langkah-langkah Praktikum
Persiapan membuat dokumen HTML dengan nama file lab4_box.html seperti berikut.
1. Membuat Box Element
Kemudian tambahkan kode untuk membuat box element dengan tag div seperti berikut.
2. CSS Float Property
Selanjutnya tambahkan deklarasi CSS pada head untuk membuat float element, seperti berikut.
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Box Element</title>
    <style>
        div {
            float: left;
            padding: 10px;
        }

        .div1 {
            background: red;
        }

        .div2 {
            background: yellow;
        }

        .div3 {
            background: green;
        }
    </style>
</head>
<body>
    <header>
        <h1>Box Element</h1>
    </header>

    <section>
        <div class="div1">Div 1</div>
        <div class="div2">Div 2</div>
        <div class="div3">Div 3</div>
    </section>
</body>
</html>
```
Hasilnya :

![gambar](https://github.com/andreanbadeh/Lab4Web/blob/bbb3fe82e45aa8f7e7731ad5ee152b00a160942c/image/Screenshot%20from%202025-10-15%2018-22-27.png)

3. Mengatur Clearfix Element
Clearfix digunakan untuk mengatur element setelah float element. Property clear digunakan untuk mengaturnya.
Tambahkan element div lainnya seteleah div3 seperti berikut.
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Box Element</title>
    <style>
        div {
            float: left;
            padding: 10px;
        }

        .div1 {
            background: red;
        }

        .div2 {
            background: yellow;
        }

        .div3 {
            background: green;
        }

        .div4 {
            background-color: blue;
            clear: left;
            float: none;
        }
    </style>
</head>
<body>
    <header>
        <h1>Box Element</h1>
    </header>

    <section>
        <div class="div1">Div 1</div>
        <div class="div2">Div 2</div>
        <div class="div3">Div 3</div>
        <div class="div4">Div 4</div>
    </section>
</body>
</html>
```

Hasilnya :

![gambar](https://github.com/andreanbadeh/Lab4Web/blob/a36089045570fb88111e6576aa8349f0d85e9515/image/Screenshot%20from%202025-10-15%2018-26-07.png)

# Membuat Layout Sederhana
Kita akan membuat layout web sederhana seperti gambar berikut. Buat folder baru dengan nama lab4_layout, kemudian buatlah file baru didalamnya dengan nama
home.html, dan file css dengan nama style.css.
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Layout Sederhana</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <div id="container">
    </div>

    <header>
        <h1>Layout Sederhana</h1>
    </header>

    <nav>
        <a href="home.html" class="active">Home</a>
        <a href="artikel.html">Artikel</a>
        <a href="about.html">About</a>
        <a href="kontak.html">Kontak</a>
    </nav>

    <section id="hero"></section>
    <section id="wrapper">
        <section id="main"></section>
        <aside id="sidebar"></aside>
    </section>

    <footer>
        <p>&copy; 2021 - Universitas Pelita Bangsa</p>
    </footer>
</body>
</html>
```

Hasilnya :

![gambar](https://github.com/andreanbadeh/Lab4Web/blob/93874f8e0f443e369ce96af819816f7c16863193/image/Screenshot%20from%202025-10-15%2018-29-22.png)

Kemudian tambahkan kode CSS untuk membuat layoutnya.
```
@import url('https://fonts.googleapis.com/css2?family=Open+Sans:ital,wght@0,300;0,400;0,600;0,700;0,800;1,300;1,400;1,600;1,700&display=swap');
@import url('https://fonts.googleapis.com/css2?family=Open+Sans+Condensed:ital,wght@0,300;0,700;1,300&display=swap');

* {
    margin: 0;
    padding: 0;
}

body {
    line-height: 1;
    font-size: 100%;
    font-family: 'Open Sans', sans-serif;
    color: #5a5a5a;
}

#container {
    width: 980px;
    margin: 0 auto;
    box-shadow: 0 0 1em #cccccc;
}

header {
    padding: 20px;
}

header h1 {
    margin: 20px 10px;
    color: #b5b5b5;
}
```

Hasilnya : 

![gambar](https://github.com/andreanbadeh/Lab4Web/blob/4e3db7a48d59e9f14cbed425b7d25e9b08bbbd66/image/Screenshot%20from%202025-10-15%2018-33-31.png)

4. Membuat Navigasi
Kemudian selanjutnya mengatur navigasi.
```
@import url('https://fonts.googleapis.com/css2?family=Open+Sans:ital,wght@0,300;0,400;0,600;0,700;0,800;1,300;1,400;1,600;1,700;1,800&display=swap');
@import url('https://fonts.googleapis.com/css2?family=Open+Sans+Condensed:ital,wght@0,300;0,700;1,300&display=swap');

* {
    margin: 0;
    padding: 0;
}

body {
    line-height: 1;
    font-size: 100%;
    font-family: 'Open Sans', sans-serif;
    color: #5a5a5a;
}

#container {
    width: 980px;
    margin: 0 auto;
    box-shadow: 0 0 1em #cccccc;
}

header {
    padding: 20px;
}

header h1 {
    margin: 20px 10px;
    color: #b5b5b5;
}

nav {
    display: block;
    background-color: #1f5faa;
}

nav a {
    padding: 15px 30px;
    display: inline-block;
    color: #ffffff;
    font-size: 14px;
    text-decoration: none;
    font-weight: bold;
}

nav a.active,
nav a:hover {
    background-color: #2b83ea;
}
```

Hasilnya :

![gambar](https://raw.githubusercontent.com/M-Rakha/Lab4Web/75989d3deaecfd8262c9fab283925b90f886f5fa/Cuplikan%20layar%202025-10-14%20103338.png)

5. Membuat Hero Panel.
Selanjutnya membuat hero panel. Tambahkan kode HTML dan CSS seperti berikut.

![gambar](https://raw.githubusercontent.com/M-Rakha/Lab4Web/beb1e9efd51652b1a8eeb2d39f4997da3137dafc/code4html.png)

![gambar](https://raw.githubusercontent.com/M-Rakha/Lab4Web/beb1e9efd51652b1a8eeb2d39f4997da3137dafc/code4css.png)

Hasilnya :

![gambar](https://raw.githubusercontent.com/M-Rakha/Lab4Web/beb1e9efd51652b1a8eeb2d39f4997da3137dafc/Cuplikan%20layar%202025-10-14%20111044.png)

6. Mengatur Layout Main dan Sidebar
Selanjutnya mengatur main content dan sidebar, tambahkan CSS float.
7. Membuat Sidebar Widget
Kemudian selanjutnya menambahkan element lain dalam sidebar.

![gambar](https://raw.githubusercontent.com/M-Rakha/Lab4Web/6f13a67b7e6e222ac4065429adcfb80290b0c8d4/Cuplikan%20layar%202025-10-14%20230740.png)

![gambar](https://raw.githubusercontent.com/M-Rakha/Lab4Web/6f13a67b7e6e222ac4065429adcfb80290b0c8d4/Cuplikan%20layar%202025-10-14%20231023.png)

Hasilnya :

![gambar](https://raw.githubusercontent.com/M-Rakha/Lab4Web/6f13a67b7e6e222ac4065429adcfb80290b0c8d4/Cuplikan%20layar%202025-10-14%20231114.png)

8. Mengatur Footer
Selanjutnya mengatur tampilan footer. Tambahkan CSS untuk footer.
Menambahkan Elemen lainnya pada Main Content

![gambar](https://raw.githubusercontent.com/M-Rakha/Lab4Web/12d6fbb00063df042e3215f1ea8ee16bc1cd05a0/Cuplikan%20layar%202025-10-14%20231603.png)

![gambar](https://raw.githubusercontent.com/M-Rakha/Lab4Web/12d6fbb00063df042e3215f1ea8ee16bc1cd05a0/Cuplikan%20layar%202025-10-14%20231747.png)

Hasilnya : 

![gambar](https://raw.githubusercontent.com/M-Rakha/Lab4Web/12d6fbb00063df042e3215f1ea8ee16bc1cd05a0/Cuplikan%20layar%202025-10-14%20231821.png)

SELESAI.

SOAL :

![gambar](https://raw.githubusercontent.com/M-Rakha/Lab4Web/e5bada50c537c9cb8aab323c78be291fb0a12a7b/Cuplikan%20layar%202025-10-14%20232155.png)

JAWABAN :

![gambar](https://raw.githubusercontent.com/M-Rakha/Lab4Web/c032fbecf6226ebd0f19445b167db11328e33795/code5html.png)

![gambar](https://raw.githubusercontent.com/M-Rakha/Lab4Web/c032fbecf6226ebd0f19445b167db11328e33795/code6html.png)

![gambar](https://raw.githubusercontent.com/M-Rakha/Lab4Web/c032fbecf6226ebd0f19445b167db11328e33795/Cuplikan%20layar%202025-10-14%20233255.png)

![gambar](https://raw.githubusercontent.com/M-Rakha/Lab4Web/c032fbecf6226ebd0f19445b167db11328e33795/Cuplikan%20layar%202025-10-14%20233306.png)
