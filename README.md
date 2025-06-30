# BlackFone
Servicio Tecnico
<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css">
    <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;500&display=swap" rel="stylesheet">
    <title>BlackFone - Servicio Técnico</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <header>
        <div class="hero">
            <h1>BlackFone</h1>
            <p>Servicio técnico confiable al mejor precio</p>
            <a href="https://wa.me/543517676332" class="btn-whatsapp">Cotizá por WhatsApp</a>
        </div>
    </header>

    <section class="services">
        <h2>Servicios Ofrecidos</h2>
        <div class="service-card">
            <i class="fas fa-mobile-alt"></i>
            <h3>Cambio de pantalla</h3>
        </div>
        <div class="service-card">
            <i class="fas fa-battery-half"></i>
            <h3>Cambio de batería</h3>
        </div>
        <div class="service-card">
            <i class="fas fa-tools"></i>
            <h3>Diagnóstico sin cargo</h3>
        </div>
    </section>

    <section class="gallery">
        <h2>Galería de Trabajos</h2>
        <div class="gallery-images">
            <!-- Imágenes de trabajos -->
        </div>
    </section>

    <footer>
        <p>Contacto: guevarajavier2224@gmail.com | Dirección: Cordoba Capital</p>
        <div class="socials">
            <a href="#"><i class="fab fa-facebook"></i></a>
            <a href="#"><i class="fab fa-instagram"Blackfone.cba</i></a>
        </div>
    </footer>

    <div class="back-to-top" onclick="scrollToTop()">
        <i class="fas fa-chevron-up"></i>
    </div>

    <script src="script.js"></script>
</body>body {
    font-family: 'Poppins', sans-serif;
    margin: 0;
    padding: 0;
    background-color: #0d0d0d;
    color: #f1f1f1;
}

.hero {
    text-align: center;
    padding: 50px 20px;
    background-color: #0d0d0d;
}

.btn-whatsapp {
    background-color: #facc15;
    color: #0d0d0d;
    padding: 10px 20px;
    text-decoration: none;
    border-radius: 5px;
}

.services {
    padding: 20px;
    text-align: center;
}

.service-card {
    display: inline-block;
    margin: 20px;
    padding: 20px;
    background-color: #1a1a1a;
    border-radius: 10px;
    width: 200px;
}

.gallery {
    padding: 20px;
}

footer {
    text-align: center;
    padding: 20px;
    background-color: #1a1a1a;
}

.socials a {
    color: #f1f1f1;
    margin: 0 10px;
}

.back-to-top {
    position: fixed;
    bottom: 20px;
    right: 20px;
    background-color: #facc15;
    border-radius: 50%;
    padding: 10px;
    cursor: pointer;
}

</html>function scrollToTop() {
    window.scrollTo({
        top: 0,
        behavior: 'smooth'
    });
}

// Animación de entrada
window.addEventListener('scroll', function() {
    const sections = document.querySelectorAll('section');
    sections.forEach(section => {
        const sectionTop = section.getBoundingClientRect().top;
        const windowHeight = window.innerHeight;
        if (sectionTop < windowHeight - 100) {
            section.classList.add('fade-in');
        }
    });
});

