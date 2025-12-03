<!DOCTYPE html>
<html lang="pt">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Minha Página Web</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f4f4f4;
        }
        header {
            background-color: #4CAF50;
            color: white;
            padding: 20px 10px;
            text-align: center;
        }
        nav {
            background-color: #333;
        }
        nav a {
            color: white;
            padding: 14px 20px;
            display: inline-block;
            text-decoration: none;
        }
        nav a:hover {
            background-color: #575757;
        }
        main {
            padding: 20px;
        }
        footer {
            background-color: #333;
            color: white;
            text-align: center;
            padding: 10px;
            position: fixed;
            bottom: 0;
            width: 100%;
        }
    </style>
</head>
<body>

    <header>
        <h1>Bem-vindo à Minha Página</h1>
    </header>

    <nav>
        <a href="#home">Home</a>
        <a href="#sobre">Sobre</a>
        <a href="#contato">Contato</a>
    </nav>

    <main>
        <section id="home">
            <h2>Home</h2>
            <p>Esta é a página inicial do meu site.</p>
        </section>

        <section id="sobre">
            <h2>Sobre</h2>
            <p>Aqui você pode falar um pouco sobre você ou sobre o seu projeto.</p>
        </section>

        <section id="contato">
            <h2>Contato</h2>
            <p>Email: exemplo@dominio.com</p>
        </section>
    </main>

    <footer>
        &copy; 2025 Minha Página Web
    </footer>

</body>
</html>