### Hi there 👋
- 🔭 Em busca da primeira oportunidade de emprego em setores relacionados á tecnologia.
- 🌱 Estudante de ciência da computação
- 💬 Contate-me: caio.friedemann@outlook.com

<!DOCTYPE html>
<html>
<head>
  <title>Meu Perfil do GitHub</title>
  <link rel="stylesheet" href="styles.css">
  <script src="script.js"></script>
</head>
<body>
  <header>
    <h1>Meu Perfil do GitHub</h1>
  </header>
  
  <main>
    <section>
      <h2>Informações do Perfil</h2>
      <div id="profile-info">
        <img id="avatar" src="avatar.jpg" alt="Avatar">
        <div id="user-details">
          <h3 id="username">Seu Nome de Usuário</h3>
          <p id="location">Sua Localização</p>
          <p id="bio">Sua Biografia</p>
          <p id="public-repos">Repositórios Públicos: <span>0</span></p>
          <p id="followers">Seguidores: <span>0</span></p>
          <p id="following">Seguindo: <span>0</span></p>
        </div>
      </div>
    </section>
    
    <section>
      <h2>Repositórios</h2>
      <ul id="repo-list"></ul>
    </section>
  </main>
  
  <footer>
    <p>© 2023 Seu Nome. Todos os direitos reservados.</p>
  </footer>
  
  <script>
    // Script para preencher as informações do perfil
    const apiUrl = 'https://api.github.com/users/seu-usuario'; // Substitua "seu-usuario" pelo seu nome de usuário do GitHub
    
    fetch(apiUrl)
      .then(response => response.json())
      .then(data => {
        document.getElementById('avatar').src = data.avatar_url;
        document.getElementById('username').textContent = data.login;
        document.getElementById('location').textContent = data.location;
        document.getElementById('bio').textContent = data.bio;
        document.getElementById('public-repos').querySelector('span').textContent = data.public_repos;
        document.getElementById('followers').querySelector

      <ul>
        <li><a href="https://github.com/seu-usuario/repositorio1">Repositório 1</a></li>
        <li><a href="https://github.com/seu-usuario/repositorio2">Repositório 2</a></li>
        <li><a href="https://github.com/seu-usuario/repositorio3">Repositório 3</a></li>
      </ul>
    </section>
  </main>
  
  <footer>
    <p>© 2023 Seu Nome. Todos os direitos reservados.</p>
  </footer>
</body>
</html>
