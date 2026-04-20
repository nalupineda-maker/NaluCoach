# NaluCoach<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Nalu Coach | Espacio de Transformación</title>
    <link href="https://fonts.googleapis.com/css2?family=DM+Sans:wght@400;500&family=Cormorant+Garamond:ital,wght@0,600;1,500&display=swap" rel="stylesheet">
    <style>
        :root {
            --primary: #d4a373; /* Tono tierra suave */
            --secondary: #faedcd; /* Crema/Arena */
            --accent: #bc6c25; /* Terracota */
            --text: #4a4a4a;
            --white: #fefae0;
            --font-serif: 'Cormorant Garamond', serif;
            --font-sans: 'DM Sans', sans-serif;
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: var(--font-sans);
            color: var(--text);
            background-color: var(--white);
            line-height: 1.7;
        }

        /* Header Estilo Minimal */
        header {
            padding: 2rem;
            text-align: center;
            background-color: transparent;
        }

        .logo {
            font-family: var(--font-serif);
            font-size: 2.2rem;
            color: var(--accent);
            text-decoration: none;
            letter-spacing: 1px;
        }

        /* Hero Section - Enfoque Visual */
        .hero {
            display: flex;
            flex-direction: column;
            align-items: center;
            padding: 4rem 10%;
            text-align: center;
            background: linear-gradient(180deg, var(--white) 0%, var(--secondary) 100%);
        }

        .hero-img {
            width: 180px;
            height: 180px;
            border-radius: 50%;
            object-fit: cover;
            border: 5px solid white;
            margin-bottom: 2rem;
            box-shadow: 0 10px 20px rgba(0,0,0,0.05);
        }

        .hero h1 {
            font-family: var(--font-serif);
            font-size: 3rem;
            color: var(--accent);
            margin-bottom: 1rem;
            font-style: italic;
        }

        .hero p {
            max-width: 600px;
            font-size: 1.1rem;
            margin-bottom: 2rem;
        }

        /* Botones Redondeados */
        .btn {
            padding: 1.2rem 2.5rem;
            border-radius: 40px;
            text-decoration: none;
            font-weight: 500;
            transition: all 0.3s ease;
            display: inline-block;
        }

        .btn-main {
            background-color: var(--accent);
            color: white;
            box-shadow: 0 4px 15px rgba(188, 108, 37, 0.3);
        }

        .btn-main:hover {
            transform: translateY(-3px);
            background-color: var(--primary);
        }

        /* Secciones de Contenido */
        .section {
            padding: 5rem 10%;
        }

        .title-center {
            text-align: center;
            font-family: var(--font-serif);
            font-size: 2.5rem;
            margin-bottom: 3rem;
            color: var(--accent);
        }

        /* Grid de Servicios con Formas Orgánicas */
        .services-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
            gap: 2.5rem;
        }

        .service-card {
            background: white;
            padding: 3rem 2rem;
            border-radius: 60px 15px 60px 15px; /* Forma asimétrica orgánica */
            text-align: center;
            transition: 0.3s;
            border: 1px solid var(--secondary);
        }

        .service-card h3 {
            font-family: var(--font-serif);
            font-size: 1.8rem;
            margin-bottom: 1rem;
            color: var(--primary);
        }

        /* Contacto Estilo Instagram */
        .contact-box {
            background-color: var(--secondary);
            padding: 4rem 2rem;
            border-radius: 30px;
            text-align: center;
            max-width: 900px;
            margin: 0 auto;
        }

        form {
            display: grid;
            gap: 1rem;
            max-width: 500px;
            margin: 2rem auto 0;
        }

        input, textarea {
            padding: 1rem;
            border: none;
            border-radius: 15px;
            background: white;
            font-family: inherit;
        }

        footer {
            text-align: center;
            padding: 3rem;
            font-size: 0.9rem;
            color: var(--accent);
        }

        /* Animaciones */
        .fade-in {
            animation: fadeIn 1.5s ease-in;
        }

        @keyframes fadeIn {
            from { opacity: 0; transform: translateY(10px); }
            to { opacity: 1; transform: translateY(0); }
        }

        @media (max-width: 768px) {
            .hero h1 { font-size: 2.2rem; }
            .section { padding: 3rem 5%; }
        }
    </style>
</head>
<body>

    <header>
        <a href="#" class="logo">Nalu.</a>
    </header>

    <section class="hero fade-in">
        <img src="https://images.unsplash.com/photo-1544005313-94ddf0286df2?auto=format&fit=crop&q=80&w=300" alt="Nalu" class="hero-img">
        <h1>Acompañando tu despertar.</h1>
        <p>Coach de Vida y Bienestar. Te ayudo a reconectar con tu esencia y manifestar la realidad que deseas desde el amor propio.</p>
        <a href="#contacto" class="btn btn-main">Reserva tu sesión de claridad</a>
    </section>

    <section class="section" id="servicios">
        <h2 class="title-center">Programas para ti</h2>
        <div class="services-grid">
            <div class="service-card">
                <h3>Mindset & Flow</h3>
                <p>Sesiones 1:1 para romper creencias limitantes y fluir con tus proyectos.</p>
            </div>
            <div class="service-card" style="background-color: var(--primary); color: white;">
                <h3 style="color: white;">Retiros Soul</h3>
                <p>Experiencias grupales de inmersión para resetear tu energía vital.</p>
            </div>
            <div class="service-card">
                <h3>Talleres Online</h3>
                <p>Herramientas prácticas de manifestación y gestión emocional a tu ritmo.</p>
            </div>
        </div>
    </section>

    <section class="section">
        <div class="contact-box" id="contacto">
            <h2 style="font-family: var(--font-serif); font-size: 2.2rem;">¿Lista para empezar?</h2>
            <p>Cuéntame en qué punto de tu camino te encuentras.</p>
            <form id="naluForm">
                <input type="text" placeholder="Nombre completo" required>
                <input type="email" placeholder="Correo electrónico" required>
                <textarea rows="4" placeholder="¿Cómo puedo acompañarte hoy?"></textarea>
                <button type="submit" class="btn btn-main">Enviar mensaje</button>
            </form>
        </div>
    </section>

    <footer>
        <p>Hecho con amor • Nalu Coach 2026</p>
        <div style="margin-top: 1rem;">
            <small>Instagram | Spotify | Pinterest</small>
        </div>
    </footer>

    <script>
        // Manejo del formulario
        document.getElementById('naluForm').addEventListener('submit', function(e) {
            e.preventDefault();
            const btn = this.querySelector('button');
            btn.innerText = 'Enviando luz...';
            
            setTimeout(() => {
                alert('¡Mensaje recibido! Te responderé muy pronto con mucha alegría.');
                this.reset();
                btn.innerText = 'Enviar mensaje';
            }, 1800);
        });

        // Scroll suave
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function (e) {
                e.preventDefault();
                document.querySelector(this.getAttribute('href')).scrollIntoView({
                    behavior: 'smooth'
                });
            });
        });
    </script>
</body>
</html>
