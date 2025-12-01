<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Invitación a la Fiesta de la Virgen de Juquila</title>
    <link href="https://fonts.googleapis.com/css2?family=Playfair+Display:wght@700&family=Montserrat:wght@400;700&display=swap" rel="stylesheet">
    <style>
        body {
            font-family: 'Montserrat', sans-serif;
            /* URL de la imagen de fondo de la Virgen de Juquila */
            background-image: linear-gradient(to top, #fbc2eb 0%, #a6c1ee 100%);
            background-size: cover;
            background-position: center;
            background-attachment: fixed;
            color: #333;
            margin: 0;
            padding: 20px;
            display: flex;
            justify-content: center;
            align-items: center;
            min-height: 100vh;
        }
        .invitation {
            background-color: rgba(255, 255, 255, 0.95); /* Fondo blanco semi-transparente para legibilidad */
            border: 2px solid #e0c5a0;
            border-radius: 10px;
            padding: 30px 40px;
            max-width: 600px;
            text-align: center;
            box-shadow: 0 8px 16px rgba(0,0,0,0.2);
        }
        h1 {
            font-family: 'Playfair Display', serif;
            color: #8c5b2a; /* Tono dorado oscuro */
            font-size: 2.8em;
            margin-bottom: 10px;
            text-shadow: 1px 1px 2px rgba(0,0,0,0.1);
        }
        h2 {
            font-family: 'Playfair Display', serif;
            color: #4a4a4a;
            font-size: 1.5em;
            margin-top: 0;
        }
        p {
            font-size: 1.1em;
            line-height: 1.6;
            color: #333;
        }
        .details {
            background-color: #fef8f0;
            border: 1px dashed #d4b790;
            padding: 15px;
            margin: 20px 0;
            text-align: left;
            border-radius: 8px;
        }
        strong {
            color: #c58a46;
            font-weight: 700;
        }
        .prayer-btn {
            background-color: #8c5b2a;
            color: white;
            border: none;
            padding: 12px 25px;
            font-size: 1em;
            font-family: 'Montserrat', sans-serif;
            font-weight: 700;
            border-radius: 25px;
            cursor: pointer;
            transition: background-color 0.3s, transform 0.2s;
            margin-top: 20px;
        }
        .prayer-btn:hover {
            background-color: #a97a4f;
            transform: scale(1.05);
        }
        .prayer-content {
            display: none; /* Oculto por defecto */
            margin-top: 20px;
            padding: 20px;
            background-color: #fffaf2;
            border-radius: 8px;
            border: 1px solid #e0c5a0;
            text-align: center;
        }
        .prayer-content img {
            max-width: 150px;
            border-radius: 50%;
            border: 4px solid #e0c5a0;
            margin-bottom: 15px;
        }
        .prayer-content p {
            font-style: italic;
            color: #555;
            font-size: 1em;
        }
    </style>
</head>
<body>
    <div class="invitation">
        <h2>La familia <strong>Sánchez Calleja</strong> tiene el honor de invitarte</h2>
        <h2>a la celebración anual en honor a la</h2>
        <h1>Virgen de Juquila</h1>
        <p>Acompáñanos en familia a dar gracias y festejar a nuestra amada Virgen de Juquila.</p>
        
        <div class="details">
            <p><strong>Fecha:</strong> 6 de diciembre</p>
            <p><strong>Recorrido de Calenda:</strong> A las <strong>6:00 PM</strong>, recorreremos las calles de la localidad.</p>
            <p><strong>Santa Misa:</strong> A las <strong>7:00 PM</strong> en casa de la familia anfitriona.</p>
        </div>

        <p>Esperamos contar con tu presencia para compartir este día de fe y alegría.</p>
        <p><em>"Madre querida, Virgen de Juquila, ruega por nosotros."</em></p>

        <button id="prayer-toggle-btn" class="prayer-btn">Mostrar Oración e Imagen</button>

        <div id="prayer-section" class="prayer-content">
            <img src="c:\Users\marti\Downloads\c.jpg" alt="Virgen de Juquila">
            <p><strong>Oración a la Virgen de Juquila</strong></p>
            <p>"Madre Querida, Virgen de Juquila, Virgen de nuestra esperanza, tuya es nuestra vida, cuídanos de todo mal. Si en este mundo de injusticias, de miseria y pecado, ves que nuestra vida se turba, no nos abandones. Madre Querida, protege a los peregrinos, acompáñanos por todos los caminos, vela por los pobres sin sustento y el pan que se les quita retribúyeselos. Acompáñanos en toda nuestra vida y libéranos de todo tipo de pecado. Amén."</p>
        </div>
    </div>

    <script>
        const prayerBtn = document.getElementById('prayer-toggle-btn');
        const prayerSection = document.getElementById('prayer-section');

        prayerBtn.addEventListener('click', () => {
            const isHidden = prayerSection.style.display === 'none' || prayerSection.style.display === '';
            prayerSection.style.display = isHidden ? 'block' : 'none';
            prayerBtn.textContent = isHidden ? 'Ocultar Oración e Imagen' : 'Mostrar Oración e Imagen';
        });
    </script>
</body>
</html>
