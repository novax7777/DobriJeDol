<!DOCTYPE html>
<html lang="hr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>MMA Klub Dobar je dol</title>
    <style>
        * {
            box-sizing: border-box;
            margin: 0;
            padding: 0;
        }
        body {
            font-family: Arial, sans-serif;
            background-color: #0d0d0d;
            color: white;
            text-align: center;
            margin: 0;
            padding: 0;
        }
        header {
            background-color: #222;
            padding: 20px;
            font-size: 32px;
            font-weight: bold;
            letter-spacing: 2px;
            text-transform: uppercase;
        }
        .container {
            max-width: 800px;
            margin: 30px auto;
            padding: 20px;
            background-color: #1a1a1a;
            border-radius: 10px;
            box-shadow: 0 0 15px rgba(255, 0, 0, 0.5);
        }
        h2 {
            color: #e63946;
            margin-bottom: 10px;
        }
        p {
            font-size: 18px;
            line-height: 1.6;
            margin-bottom: 10px;
        }
        .btn-container {
            display: flex;
            justify-content: center;
            gap: 15px;
            margin-top: 20px;
            flex-wrap: wrap;
        }
        .btn {
            display: inline-block;
            padding: 12px 25px;
            background: linear-gradient(45deg, #e63946, #ff5733);
            color: white;
            text-decoration: none;
            font-weight: bold;
            border-radius: 5px;
            font-size: 18px;
            transition: 0.3s ease;
            cursor: pointer;
            border: none;
            width: 100%;
            max-width: 250px;
        }
        .btn:hover {
            background: linear-gradient(45deg, #ff5733, #e63946);
            transform: scale(1.05);
        }
        .message {
            display: none;
            margin-top: 20px;
            font-size: 20px;
            font-weight: bold;
            color: #ff4747;
        }
        footer {
            margin-top: 30px;
            padding: 15px;
            background-color: #222;
            font-size: 14px;
            color: #ccc;
        }

        @media (max-width: 600px) {
            header {
                font-size: 28px;
                padding: 15px;
            }
            .container {
                max-width: 95%;
                padding: 15px;
            }
            .btn-container {
                flex-direction: column;
                gap: 10px;
            }
            .btn {
                width: 100%;
                padding: 15px;
                font-size: 20px;
            }
        }
    </style>
</head>
<body>

<header>
    MMA Klub "Dobar je dol"
</header>

<div class="container">
    <h2>O nama</h2>
    <p>MMA Klub "Dobar je dol" mjesto je gdje snaga, tehnika i disciplina postaju jedno.</p>
    <p>Bilo da ste početnik ili iskusni borac, naši treneri pomoći će vam da postignete vrhunsku formu!</p>
    
    <h2>Programi treninga</h2>
    <p>🥊 Boks</p>
    <p>🥋 Brazilski jiu-jitsu</p>
    <p>🥊 Kickboxing</p>
    <p>🔥 MMA</p>
    <p>🤼‍♂️ Hrvanje</p>
    <p>🥊 Muay Thai</p>

    <h2>Kontakt</h2>
    <p>📧 Email: info@dobarjedol.com</p>
    <p>📞 Telefon: +385 91 123 4567</p>

    <div class="btn-container">
        <button class="btn" onclick="prikaziPoruku('pridruzi')">Pridruži nam se</button>
        <button class="btn" onclick="prikaziPoruku('kontakt')">Kontaktiraj nas</button>
    </div>

    <p id="pridruzi" class="message">NEMOJ MOLIM TE SE PRIDRUŽITI</p>
    <p id="kontakt" class="message">PRESTANI NAS KONTAKTIRAT NE ŽELIMO TE PRIMITI U KLUB</p>
</div>

<footer>
    © 2025 MMA Klub "Dobar je dol" - Sva prava pridržana.
</footer>

<script>
    function prikaziPoruku(id) {
        var poruka = document.getElementById(id);
        if (poruka.style.display === "none" || poruka.style.display === "") {
            poruka.style.display = "block";
        } else {
            poruka.style.display = "none";
        }
    }
</script>

</body>
</html>
