<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Biodata</title>
    <style>
        body { font-family: Arial, sans-serif; text-align: center; background-color: #1E90FF; color: white; }
        .container { max-width: 600px; margin: auto; padding: 20px; border: 1px solid #ccc; border-radius: 10px; background-color: rgba(255, 255, 255, 0.9); color: black; }
        .hidden { display: none; }
        button { margin-top: 10px; padding: 10px; cursor: pointer; }
        img { width: 150px; height: 150px; border-radius: 50%; margin-bottom: 15px; }
    </style>
</head>
<body>
    <div class="container" id="page1">
        <h2>Halaman 1: Informasi Pribadi</h2>
        <img src="profile.jpg" alt="Foto Profil">
        <p><strong>Nama:</strong> Asma Lutfi</p>
        <p><strong>Alamat:</strong> Jl. Lengaru, Palu</p>
        <p><strong>Email:</strong> asmalutfi025@gmail.com</p>
        <p><strong>No. HP:</strong> 082187937743</p>
        <button onclick="showPage(2)">Lanjut ke Halaman 2</button>
    </div>
    <div class="container hidden" id="page2">
    <h2>Halaman 2: Pendidikan & Keterampilan</h2>
    <img src="education.jpg" alt="Pendidikan">
    <p><strong>Pendidikan:</strong> S1 Sistem Informasi, Universitas Tadulako</p>
    <button onclick="showPage(1)">Kembali ke Halaman 1</button>
    </div>
    <script>
    function showPage(page) {
        document.getElementById('page1').classList.add('hidden');
        document.getElementById('page2').classList.add('hidden');
        document.getElementById('page' + page).classList.remove('hidden');
    }
    </script>
</body>
</html>
