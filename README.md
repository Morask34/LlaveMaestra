<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Llave Maestra - Cerrajería 24h</title>
    <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@400;600;700&display=swap" rel="stylesheet">
    <style>
        :root {
            --primary-color: #007bff; /* Azul vibrante */
            --secondary-color: #6c757d; /* Gris para textos secundarios */
            --dark-color: #343a40; /* Casi negro para fondos */
            --light-color: #f8f9fa; /* Blanco roto para fondos claros */
            --white-color: #ffffff;
            --success-color: #28a745; /* Verde para éxito */
            --danger-color: #dc3545; /* Rojo para alertas */
        }

        body {
            font-family: 'Poppins', sans-serif;
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            line-height: 1.6;
            color: var(--dark-color);
            background-color: var(--light-color);
        }

        header {
            background-color: var(--dark-color);
            color: var(--white-color);
            padding: 1rem 0;
            text-align: center;
            box-shadow: 0 2px 5px rgba(0,0,0,0.2);
        }

        header h1 {
            margin: 0;
            font-size: 2.8em;
            color: var(--primary-color);
        }

        header p {
            margin: 0.5rem 0;
            font-size: 1.2em;
        }

        .container {
            width: 90%;
            max-width: 1200px;
            margin: auto;
            overflow: hidden;
            padding: 2rem 0;
        }

        .hero {
            background: linear-gradient(rgba(0, 0, 0, 0.6), rgba(0, 0, 0, 0.6)), url('https://via.placeholder.com/1500x500?text=Tu+Imagen+de+Cerrajería') no-repeat center center/cover;
            color: var(--white-color);
            text-align: center;
            padding: 5rem 0;
            margin-bottom: 2rem;
            border-radius: 8px;
        }

        .hero h2 {
            font-size: 3em;
            margin-bottom: 1rem;
            color: var(--primary-color);
        }

        .hero p {
            font-size: 1.5em;
            margin-bottom: 2rem;
        }

        .btn {
            display: inline-block;
            background-color: var(--primary-color);
            color: var(--white-color);
            padding: 0.8rem 2rem;
            border-radius: 50px;
            text-decoration: none;
            font-size: 1.1em;
            transition: background-color 0.3s ease, transform 0.2s ease;
            margin: 0.5rem;
            border: none;
            cursor: pointer;
        }

        .btn:hover {
            background-color: #0056b3; /* Un azul más oscuro */
            transform: translateY(-3px);
        }

        .btn-danger {
            background-color: var(--danger-color);
        }
        .btn-danger:hover {
            background-color: #c82333;
        }

        .btn-success {
            background-color: var(--success-color);
        }
        .btn-success:hover {
            background-color: #218838;
        }

        .section-title {
            text-align: center;
            font-size: 2.5em;
            margin-bottom: 2rem;
            color: var(--dark-color);
            position: relative;
            padding-bottom: 10px;
        }

        .section-title::after {
            content: '';
            position: absolute;
            left: 50%;
            bottom: 0;
            transform: translateX(-50%);
            width: 80px;
            height: 4px;
            background-color: var(--primary-color);
            border-radius: 2px;
        }

        .services, .contact {
            background-color: var(--white-color);
            padding: 2rem;
            border-radius: 8px;
            box-shadow: 0 4px 10px rgba(0,0,0,0.1);
            margin-bottom: 2rem;
        }

        .services-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
            gap: 1.5rem;
        }

        .service-item {
            background-color: var(--light-color);
            padding: 1.5rem;
            border-radius: 8px;
            text-align: center;
            transition: transform 0.3s ease, box-shadow 0.3s ease;
            border: 1px solid #e0e0e0;
        }

        .service-item:hover {
            transform: translateY(-5px);
            box-shadow: 0 6px 15px rgba(0,0,0,0.15);
        }

        .service-item h3 {
            color: var(--primary-color);
            font-size: 1.4em;
            margin-bottom: 0.8rem;
        }

        .service-item p {
            color: var(--secondary-color);
        }

        .social-buttons {
            text-align: center;
            margin-top: 2rem;
        }

        .social-buttons a {
            display: inline-block;
            font-size: 2em;
            color: var(--dark-color);
            margin: 0 0.7rem;
            transition: color 0.3s ease;
        }

        .social-buttons a:hover {
            color: var(--primary-color);
        }

        footer {
            background-color: var(--dark-color);
            color: var(--white-color);
            text-align: center;
            padding: 1.5rem 0;
            margin-top: 2rem;
        }

        /* Responsive adjustments */
        @media (max-width: 768px) {
            header h1 {
                font-size: 2em;
            }
            .hero h2 {
                font-size: 2.2em;
            }
            .hero p {
                font-size: 1.2em;
            }
            .btn {
                padding: 0.7rem 1.5rem;
                font-size: 1em;
            }
            .section-title {
                font-size: 2em;
            }
        }

        @media (max-width: 480px) {
            .btn {
                display: block;
                width: 80%;
                margin: 0.5rem auto;
            }
        }
    </style>
</head>
<body>

    <header>
        <h1>Llave Maestra</h1>
        <p>Tu Cerrajería de Confianza</p>
        <p>¡Abierto las 24 horas del día!</p>
    </header>

    <div class="hero">
        <div class="container">
            <h2>¿Problemas con tus llaves? ¡Estamos aquí para ayudarte!</h2>
            <p>Servicio de cerrajería rápido, seguro y disponible las 24h.</p>
            <a href="tel:6711132883" class="btn btn-danger">Llamada de Emergencia</a>
            <a href="#cotizacion" class="btn btn-success">Solicitar Cotización</a>
        </div>
    </div>

    <div class="container">
        <hr>
        <section class="services">
            <h2 class="section-title">Nuestros Servicios</h2>
            <div class="services-grid">
                <div class="service-item">
                    <h3>Apertura de Puertas</h3>
                    <p>Acceso rápido a tu hogar, oficina o vehículo sin daños.</p>
                </div>
                <div class="service-item">
                    <h3>Cambio y Reparación de Cerraduras</h3>
                    <p>Instalación y mantenimiento de cerraduras de alta seguridad.</p>
                </div>
                <div class="service-item">
                    <h3>Duplicado de Llaves</h3>
                    <p>Copias exactas para todo tipo de llaves.</p>
                </div>
            </div>
        </section>

        <hr>

        <section id="cotizacion" class="contact">
            <h2 class="section-title">Solicita una Cotización vía WhatsApp</h2>
            <p style="text-align: center; margin-bottom: 1.5rem; color: var(--secondary-color);">
                Completa el formulario y haz clic en "Enviar por WhatsApp" para enviarnos tu solicitud directamente.
            </p>
            <form id="quoteForm" style="max-width: 600px; margin: auto;">
                <div style="margin-bottom: 1rem;">
                    <label for="name" style="display: block; margin-bottom: 0.5rem; font-weight: 600;">Nombre completo:</label>
                    <input type="text" id="name" name="name" required style="width: 100%; padding: 0.8rem; border: 1px solid #ccc; border-radius: 4px; box-sizing: border-box;">
                </div>
                <div style="margin-bottom: 1rem;">
                    <label for="email" style="display: block; margin-bottom: 0.5rem; font-weight: 600;">Correo electrónico:</label>
                    <input type="email" id="email" name="email" required style="width: 100%; padding: 0.8rem; border: 1px solid #ccc; border-radius: 4px; box-sizing: border-box;">
                </div>
                <div style="margin-bottom: 1rem;">
                    <label for="phone" style="display: block; margin-bottom: 0.5rem; font-weight: 600;">Número de teléfono:</label>
                    <input type="tel" id="phone" name="phone" required style="width: 100%; padding: 0.8rem; border: 1px solid #ccc; border-radius: 4px; box-sizing: border-box;">
                </div>
                <div style="margin-bottom: 1rem;">
                    <label for="service" style="display: block; margin-bottom: 0.5rem; font-weight: 600;">Tipo de Servicio:</label>
                    <select id="service" name="service" required style="width: 100%; padding: 0.8rem; border: 1px solid #ccc; border-radius: 4px; box-sizing: border-box;">
                        <option value="">Selecciona un servicio</option>
                        <option value="Apertura de Puertas">Apertura de Puertas</option>
                        <option value="Cambio/Reparacion de Cerradura">Cambio/Reparación de Cerradura</option>
                        <option value="Duplicado de Llaves">Duplicado de Llaves</option>
                    </select>
                </div>
                <div style="margin-bottom: 1rem;">
                    <label for="message" style="display: block; margin-bottom: 0.5rem; font-weight: 600;">Mensaje / Detalles:</label>
                    <textarea id="message" name="message" rows="5" required style="width: 100%; padding: 0.8rem; border: 1px solid #ccc; border-radius: 4px; box-sizing: border-box; resize: vertical;"></textarea>
                </div>
                <button type="submit" class="btn" style="width: 100%;">Enviar Solicitud por WhatsApp</button>
            </form>
            <p style="text-align: center; margin-top: 1rem; color: var(--secondary-color); font-size: 0.9em;">
                Se abrirá WhatsApp con los detalles de tu solicitud para que puedas enviárnosla.
            </p>
        </section>

        <hr>

        <section class="social-buttons">
            <h2 class="section-title">Síguenos en Redes Sociales</h2>
            <div>
                <a href="https://wa.me/6711132883" target="_blank" aria-label="WhatsApp">
                    <img src="https://img.icons8.com/ios-filled/50/000000/whatsapp--v1.png" alt="WhatsApp" width="50" height="50">
                </a>
                <a href="https://www.instagram.com/Llavemaestra247h" target="_blank" aria-label="Instagram">
                    <img src="https://img.icons8.com/ios-filled/50/000000/instagram-new--v1.png" alt="Instagram" width="50" height="50">
                </a>
                </div>
        </section>
    </div>

    <footer>
        <p>&copy; 2025 Llave Maestra. Todos los derechos reservados.</p>
        <p>¡Tu seguridad es nuestra prioridad 24/7!</p>
    </footer>

    <script>
        // Smooth scrolling for anchor links
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function (e) {
                e.preventDefault();

                document.querySelector(this.getAttribute('href')).scrollIntoView({
                    behavior: 'smooth'
                });
            });
        });

        // Function to send form data to WhatsApp
        const quoteForm = document.getElementById('quoteForm');
        if (quoteForm) {
            quoteForm.addEventListener('submit', function(e) {
                e.preventDefault(); // Prevent default form submission

                const name = document.getElementById('name').value;
                const email = document.getElementById('email').value;
                const phone = document.getElementById('phone').value;
                const service = document.getElementById('service').value;
                const message = document.getElementById('message').value;

                // IMPORTANT: Replace '525512345678' with your actual WhatsApp number, including country code
                const yourWhatsAppNumber = '6711132883'; 

                // Construct the WhatsApp message text
                // %0A creates a new line in WhatsApp
                let whatsappMessage = `*Nueva Solicitud de Cotización Llave Maestra*\n\n`;
                whatsappMessage += `*Nombre:* ${name}\n`;
                whatsappMessage += `*Email:* ${email}\n`;
                whatsappMessage += `*Teléfono:* ${phone}\n`;
                whatsappMessage += `*Servicio:* ${service}\n`;
                whatsappMessage += `*Detalles:* ${message}\n\n`;
                whatsappMessage += `_Este mensaje fue enviado desde el formulario de tu sitio web._`;

                // Encode the message for a URL
                const encodedMessage = encodeURIComponent(whatsappMessage);

                // Create the WhatsApp URL
                const whatsappUrl = `https://wa.me/${yourWhatsAppNumber}?text=${encodedMessage}`;

                // Open WhatsApp in a new tab/window
                window.open(whatsappUrl, '_blank');

                // Optionally, clear the form after opening WhatsApp
                quoteForm.reset();

                // You might also add a small message on the page indicating WhatsApp is opening
                alert('¡Estamos preparando tu mensaje de WhatsApp! Por favor, envíalo una vez que se abra.');
            });
        }
    </script>

</body>
</html>
