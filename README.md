=<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>DarkCyber App Store</title>
    <link href="https://fonts.googleapis.com/css2?family=Orbitron:wght@400;700&family=Roboto:wght@300;400;700&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/sweetalert2@11/dist/sweetalert2.min.css">
    <script src="https://cdn.jsdelivr.net/npm/sweetalert2@11"></script>
    <style>
        /* Tema DarkCyber */
        body {
            margin: 0;
            padding: 0;
            background: #0d1117;
            color: #c9d1d9;
            font-family: 'Roboto', sans-serif;
        }

        /* Splash Screen */
        #splash {
            background: linear-gradient(135deg, #6f42c1, #1f2937);
            height: 100vh;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            text-align: center;
            color: #fff;
            font-family: 'Orbitron', sans-serif;
            position: absolute;
            width: 100%;
            top: 0;
            left: 0;
            z-index: 10;
            animation: fadeOut 3s ease-in-out forwards;
        }

        #splash h1 {
            font-size: 3rem;
        }

        #splash p {
            margin-top: 10px;
            font-size: 1.2rem;
        }

        @keyframes fadeOut {
            0% { opacity: 1; }
            100% { opacity: 0; visibility: hidden; }
        }

        /* Header */
        header {
            display: flex;
            justify-content: space-between;
            align-items: center;
            background: #161b22;
            padding: 10px 20px;
        }

        header h1 {
            font-family: 'Orbitron', sans-serif;
            color: #6f42c1;
            font-size: 1.8rem;
        }

        nav a {
            text-decoration: none;
            color: #c9d1d9;
            margin: 0 10px;
            font-size: 1rem;
        }

        nav a:hover {
            color: #6f42c1;
        }

        /* Carrossel */
        .carousel {
            display: flex;
            overflow-x: auto;
            scroll-behavior: smooth;
            padding: 20px;
            gap: 20px;
        }

        .carousel img {
            width: 300px;
            height: 200px;
            border-radius: 10px;
            border: 2px solid #6f42c1;
            transition: transform 0.3s;
        }

        .carousel img:hover {
            transform: scale(1.1);
        }

        /* Apps */
        .apps {
            padding: 20px;
        }

        .apps h2 {
            font-family: 'Orbitron', sans-serif;
            text-align: center;
            margin-bottom: 20px;
        }

        .app-category {
            margin-bottom: 30px;
        }

        .app-category h3 {
            font-size: 1.5rem;
            color: #6f42c1;
            margin-bottom: 10px;
        }

        .app-list {
            display: flex;
            gap: 20px;
            flex-wrap: wrap;
        }

        .app-card {
            background: #161b22;
            border: 1px solid #6f42c1;
            border-radius: 8px;
            padding: 15px;
            width: 300px;
            text-align: center;
        }

        .app-card h4 {
            font-size: 1.2rem;
            margin-bottom: 10px;
            
            .app-card .btn {
            background: #6f42c1;
            color: #fff;
            text-decoration: none;
            padding: 8px 15px;
            border-radius: 4px;
            font-size: 0.9rem;
        }

        /* Testemunhos */
        .testimonials {
            background: #161b22;
            padding: 20px;
        }

        .testimonials h2 {
            font-family: 'Orbitron', sans-serif;
            text-align: center;
            margin-bottom: 20px;
        }

        .testimonial {
            text-align: center;
            margin-bottom: 20px;
        }

        .testimonial p {
            font-size: 1rem;
            color: #8b949e;
        }

        .testimonial span {
            font-size: 0.9rem;
            color: #6f42c1;
        }

        /* Footer */
        footer {
            background: #0d1117;
            text-align: center;
            padding: 10px 0;
            font-size: 0.9rem;
        }

        footer a {
            color: #6f42c1;
            text-decoration: none;
            margin: 0 5px;
        }

        footer a:hover {
            text-decoration: underline;
        }
    </style>
</head>
<body>
    <!-- Splash Screen -->
    <div id="splash">
        <h1>TV PREMIUM APK App Store</h1>
        <p>Carregando...</p>
    </div>

    <!-- Conteúdo Principal -->
    <header>
        <h1>TV PREMIUM 📺</h1>
        <nav>
            <a href="#apps">Apps</a>
            <a href="#testimonials">Depoimentos</a>
            <a href="#footer">Contato</a>
        </nav>
    </header>

    <!-- Carrossel de Destaques -->
    <section class="carousel">
        <img src="https://gtec.gerenciamento.pro/controler/arquivos/Promo.jpg" alt="App 1">
        <img src="https://via.placeholder.com/300x200?text=App+2" alt="App 2">
        <img src="https://via.placeholder.com/300x200?text=App+3" alt="App 3">
        <img src="https://gtec.gerenciamento.pro/controler/arquivos/IMG.jpg" alt="App 4">
    </section>

    <!-- Seção de Apps -->
    <section class="apps" id="apps">
        <h2>Aplicativos</h2>
        <div class="app-category">
            <h3>Segurança</h3>
            <div class="app-list">
                <div class="app-card">
                    <h4>APK TV 1</h4>
                    <p>Proteção máxima.</p>
                    <a href="https://dl.ntdev.in/64444" class="btn">Baixar</a>
                </div>
                <div class="app-card">
                    <h4>APK TOP 5</h4>
                    <p>Privacidade garantida.</p>
                    <a href="#" class="btn">Baixar</a>
                </div>
                <div class="app-card">
                    <h4>APK TOP 2</h4>
                    <p>Privacidade garantida.</p>
                    <a href="#" class="btn">Baixar</a>
                </div>
            </div>
        </div>
        <div class="app-category">
            <h3>Entretenimento</h3>
            <div class="app-list">
                <div class="app-card">
                    <h4>APK PRO</h4>
                    <p>Vídeos em alta qualidade.</p>
                    <a href="#" class="btn">Baixar</a>
                </div>
                <div class="app-card">
                    <h4>GameBoost</h4>
                    <p>Otimização para jogos.</p>
                    <a href="#" class="btn">Baixar</a>
                </div>
            </div>
        </div>
    </section>

    <!-- Depoimentos -->
    <section class="testimonials" id="testimonials">
        <h2>O que nossos usuários dizem</h2>
        <div class="testimonial">
            <p>"A melhor loja de apps que já usei. Interface incrível e apps confiáveis!"</p>
            <span>- João Silva</span>
        </div>
        <div class="testimonial">
            <p>"Minha experiência foi excelente! Recomendo a todos."</p>
            <span>- Maria Oliveira</span>
        </div>
    </section>

    <!-- Rodapé -->
    <footer id="footer">
        <p>© 2024 TV PREMIUM. Todos os direitos reservados.</p>
        <p>
            <a href="#">Facebook</a> | 
            <a href="#">Twitter</a> | 
            <a href="#">Instagram</a>
        </p>
    </footer>

    <script>
        // Ocultar Splash Screen após carregar
        // Ocultar Splash Screen após carregar
window.addEventListener('load', () => {
    const splash = document.getElementById('splash');
    setTimeout(() => {
        splash.style.display = 'none';

        // SweetAlert de Boas-Vindas
        Swal.fire({
            title: 'Bem-vindo!',
            text: 'Explore os melhores apps agora mesmo!',
            icon: 'info',
            confirmButtonText: 'OK',
            background: '#161b22',
            color: '#c9d1d9'
        });
    }, 3000); // Duração do Splash ajustada para 5 segundos
});
    </script>
</body>
</html>
