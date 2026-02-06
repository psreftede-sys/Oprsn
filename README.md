<!DOCTYPE html>
<html lang="id">
<head>
    <meta charset="UTF-8">
    <title>Kenangan Isi Kelas</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background: linear-gradient(135deg, #1e3c72, #2a5298);
            color: white;
            text-align: center;
            padding: 40px;
        }
        .card {
            background: rgba(0,0,0,0.4);
            padding: 25px;
            border-radius: 15px;
            max-width: 600px;
            margin: auto;
        }
        button {
            margin-top: 20px;
            padding: 10px 20px;
            border: none;
            border-radius: 8px;
            background: #ffd369;
            font-weight: bold;
            cursor: pointer;
        }
        button:hover {
            background: #ffb703;
        }
    </style>
</head>
<body>

    <div class="card">
        <h1>📸 Kenangan Isi Kelas</h1>
        <h3>XII IPA 2 – 2025</h3>

        <p id="kenangan">
            Hari pertama masuk kelas, masih canggung dan saling diam.
        </p>

        <button onclick="gantiKenangan()">Ganti Kenangan</button>
    </div>

    <script>
        const kenangan = [
            "Hari pertama masuk kelas, masih canggung dan saling diam.",
            "Tertawa bareng karena guru salah sebut nama.",
            "Belajar bareng menjelang ujian sampai sore.",
            "Dihukum satu kelas karena telat masuk.",
            "Momen foto bareng sebelum kelulusan."
        ];

        function gantiKenangan() {
            const random = Math.floor(Math.random() * kenangan.length);
            document.getElementById("kenangan").innerText = kenangan[random];
        }
    </script>

</body>
</html>
