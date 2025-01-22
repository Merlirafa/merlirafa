<body>
    <header>
        <h1>Rafael - Especialista em ServiceNow e Salesforce</h1>
        <p>Bem-vindo ao meu portfólio! Aqui você encontra detalhes sobre minha experiência e projetos nas áreas de tecnologia e automação.</p>
        <p>Welcome to my portfolio! Here you can find details about my experience and projects in the fields of technology and automation.</p>
    </header>
    <nav>
        <ul>
            <li><a href="about">Sobre Mim</a></li>
            <li><a href="projects">Projetos</a></li>
            <li><a href="contact">Contato</a></li>
        </ul>
    </nav>

    <section id="about">
        <h2>Sobre Mim</h2>
        <p>Sou formado em Análise e Desenvolvimento de Sistemas pela UMC Villa Lobos, com experiência em consultoria e análise de UX. Trabalhei em empresas como B3 e Alpar, atuando em projetos inovadores como a implementação de um chatbot integrado ao MS Luis.</p>
        <p>Certificações: UX Writing, ServiceNow VA, System Administrator, DataCloud, CRM Analytics e Marketing Cloud.</p>
    </section>

    <section id="projects">
        <h2>Projetos</h2>

        <h3>ServiceNow</h3>
        <p>Exemplo de automação com Scripted REST API:</p>
        <pre><code>(function process(request, response) {  
    var data = {  
        message: "Hello, " + request.queryParams.name || "World!"  
    };  
    response.setBody(data);  
})(request, response);
        </code></pre>

        <h3>Salesforce</h3>
        <p>Exemplo de trigger em Apex:</p>
        <pre><code>trigger UpdateContact on Account (after update) {  
    for (Account acc : Trigger.new) {  
        List<Contact> contacts = [SELECT Id, Email FROM Contact WHERE AccountId = :acc.Id];  
        for (Contact c : contacts) {  
            c.Email = acc.Email_Domain__c;  
        }  
        update contacts;  
    }  
}</code></pre>

    </section>

    <section id="contact">
        <h2>Contato</h2>
        <p>Quer entrar em contato comigo? Envie um e-mail para <strong>rafael@email.com</strong> ou acesse meu <a href="https://www.linkedin.com">LinkedIn</a>.</p>
    </section>

    <footer>
        <p>&copy; 2025 Rafael. Todos os direitos reservados.</p>
    </footer>
</body>
</html>
