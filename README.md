<!DOCTYPE html>
<html lang="tr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Senanur Yavuz - Kişisel Web Sitesi</title>
    <style>
        /* Genel Stil */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        body {
            font-family: 'Arial', sans-serif;
            line-height: 1.6;
            background: linear-gradient(to bottom, #f4f4f9, #eae6f7);
            color: #333;
            overflow-x: hidden;
        }
        header {
            background: linear-gradient(135deg, #6A1B9A, #8E24AA);
            color: white;
            padding: 60px 20px;
            text-align: center;
            clip-path: polygon(0 0, 100% 0, 100% 85%, 0 100%);
        }
        header h1 {
            font-size: 3rem;
            margin-bottom: 10px;
        }
        header p {
            font-size: 1.2rem;
        }
        nav {
            display: flex;
            justify-content: center;
            background: #333;
            padding: 10px 0;
        }
        nav a {
            color: white;
            text-decoration: none;
            margin: 0 15px;
            font-weight: bold;
            transition: color 0.3s ease, transform 0.3s ease;
        }
        nav a:hover {
            color: #8E24AA;
            transform: scale(1.1);
        }
        main {
            padding: 40px 20px;
            max-width: 1200px;
            margin: auto;
        }
        section {
            margin-bottom: 40px;
        }
        h2 {
            color: #6A1B9A;
            margin-bottom: 20px;
            text-align: center;
            font-size: 2rem;
        }

        /* Ben Kimim Bölümü */
        .about {
            background: white;
            border-radius: 8px;
            padding: 20px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
            text-align: center;
            margin: auto;
            max-width: 800px;
        }
        .about p {
            font-size: 1.2rem;
            color: #555;
            margin-bottom: 10px;
        }
        .skills {
            display: flex;
            justify-content: center;
            gap: 15px;
            margin-top: 10px;
        }
        .skill {
            background: #8E24AA;
            color: white;
            padding: 10px 20px;
            border-radius: 20px;
            font-size: 1rem;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
        }

        /* Projeler Bölümü */
        .projects {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
            gap: 20px;
        }
        .project {
            background: white;
            border-radius: 8px;
            padding: 20px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
            text-align: center;
        }
        .project h3 {
            color: #6A1B9A;
            margin-bottom: 10px;
        }
        .project p {
            color: #555;
            font-size: 1rem;
        }

        /* İletişim Bölümü */
        .contact {
            background: white;
            border-radius: 8px;
            padding: 20px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
            max-width: 800px;
            margin: auto;
        }
        .contact form {
            display: flex;
            flex-direction: column;
            gap: 15px;
        }
        .contact input, .contact textarea {
            padding: 10px;
            font-size: 1rem;
            border: 1px solid #ccc;
            border-radius: 5px;
        }
        .contact button {
            padding: 10px;
            font-size: 1rem;
            background: #6A1B9A;
            color: white;
            border: none;
            border-radius: 5px;
            cursor: pointer;
            transition: background 0.3s ease;
        }
        .contact button:hover {
            background: #8E24AA;
        }

        /* Footer */
        footer {
            background: #333;
            color: white;
            text-align: center;
            padding: 20px 0;
            margin-top: 40px;
        }
        footer p {
            font-size: 1rem;
        }
    </style>
</head>
<body>
    <header>
        <h1>Senanur Yavuz</h1>
        <p>Bilgisayar Mühendisliği Öğrencisi</p>
    </header>
    <nav>
        <a href="#about">Ben Kimim</a>
        <a href="#projects">Projelerim</a>
        <a href="#contact">İletişim</a>
    </nav>
    <main>
        <section id="about">
            <h2>Ben Kimim</h2>
            <div class="about">
                <p>Merhaba! Ben Senanur Yavuz. Bilgisayar mühendisliği öğrencisiyim ve teknolojiye olan ilgimle yazılım geliştirme üzerine çalışıyorum.</p>
                <div class="skills">
                    <div class="skill">C Programlama</div>
                    <div class="skill">Python</div>
                    <div class="skill">Web Geliştirme</div>
                </div>
            </div>
        </section>
        <section id="projects">
            <h2>Projelerim</h2>
            <div class="projects">
                <div class="project">
                    <h3>Hesap Makinesi</h3>
                    <p>Basit bir hesap makinesi uygulaması C diliyle yazılmıştır.</p>
                </div>
                <div class="project">
                    <h3>Web Sayfası Tasarımı</h3>
                    <p>HTML ve CSS kullanarak kişisel bir web sitesi tasarımı.</p>
                </div>
                <div class="project">
                    <h3>Python Veri Analizi</h3>
                    <p>Python ile veri analizi ve görselleştirme projesi.</p>
                </div>
            </div>
        </section>
        <section id="contact">
            <h2>Benimle İletişime Geçin</h2>
            <div class="contact">
                <p>Aklınıza bir proje fikri geldiyse ya da benimle iletişime geçmek isterseniz aşağıdaki formu doldurabilirsiniz:</p>
                <form>
                    <input type="text" name="name" placeholder="Adınız" required>
                    <input type="email" name="email" placeholder="E-posta Adresiniz" required>
                    <textarea name="message" rows="5" placeholder="Mesajınız" required></textarea>
                    <button type="submit">Gönder</button>
                </form>
            </div>
        </section>
    </main>
    <footer>
        <p>© 2025 Senanur Yavuz. | E-posta: senanur.y752@gmail.com</p>
    </footer>
</body>
</html>
