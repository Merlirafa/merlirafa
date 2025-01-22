<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Portfolio</title>
<link rel="stylesheet" href="style.css">
</head>
<body>
   <header>
       <h1>Welcome to My Portfolio</h1>
       <p>Explore my experience, projects, and contact details.</p>
  </header>
<nav>
      <ul>
      <li><a href="#" onclick="toggleContent(event, 'about')">Sobre Mim</a></li>
        <li><a href="#" onclick="toggleContent(event, 'projects')">Projetos</a></li>
    <li><a href="#" onclick="toggleContent(event, 'contact')">Contato</a></li>
       </ul>
   </nav>
   <section>
       <div id="about" class="hidden-content">
         <p>Sou Rafael, um profissional com experiência em tecnologia e automação...</p>
       </div>
       <div id="projects" class="hidden-content">
           <p>Aqui estão alguns dos projetos que desenvolvi, incluindo integrações e automações...</p>
        </div>
      <div id="contact" class="hidden-content">
           <p>Entre em contato comigo pelo email: rafael@example.com</p>
       </div>
   </section>
   <footer>
        <p>&copy; 2025 Rafael. Todos os direitos reservados.</p>
    </footer>
   <script>
        function toggleContent(event, id) {
            event.preventDefault();
            const content = document.getElementById(id);
            if (content.style.display === "block") {
                content.style.display = "none";
            } else {
                content.style.display = "block";
            }
        }
   </script>
</body>
</html>
