echo "# Trabalho.toji" >> README.md 
git init 
git add README.md 
git commit -m "primeiro commit" 
git branch -M main 
git remote add origin https://github.com/Apolo1Arthur/Trabalho.toji.git
 git push -u origin main

      <!DOCTYPE html>
<html lang="pt-BR">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Oprah Winfrey: Superação e Sucesso</title>
  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
    }

    body, html {
      height: 100%;
      font-family: Arial, sans-serif;
    }

    body {
      background-color: #000;
      color: #fff;
      position: relative;
      z-index: 1;
    }

    .background {
      position: fixed;
      top: 0;
      left: 0;
      width: 100%;
      height: 100%;
      z-index: -1;
      overflow: hidden;
    }

    .background img {
      width: 100%;
      height: 100%;
      object-fit: cover;
      opacity: 0.3;
    }

    .container {
      padding: 30px;
      text-align: center;
      position: relative;
      z-index: 1;
    }

    .content {
      display: none;
      background-color: rgba(0, 0, 0, 0.7);
      border-radius: 10px;
      padding: 25px;
      margin-top: 20px;
      max-width: 700px;
      margin-left: auto;
      margin-right: auto;
      text-align: left;
    }

    button {
      margin: 10px;
      padding: 12px 20px;
      border: none;
      border-radius: 8px;
      background-color: #5a2a83;
      color: white;
      font-size: 16px;
      cursor: pointer;
    }

    button:hover {
      background-color: #7635b3;
    }

    h1, h2 {
      color: #fff;
      text-shadow: 1px 1px 3px #000;
    }
  </style>
</head>
<body>

  <!-- Fundo com GIF -->
  <div class="background">
    <img id="gif" src="st1.gif" alt="Background GIF">
  </div>

  <div class="container">
    <h1>Oprah Winfrey: Superação e Sucesso</h1>

    <button onclick="showContent('intro', 'st1.gif', 'musica1.mp3')">Introdução</button>
    <button onclick="showContent('infancia', 'st2.gif', 'musica2.mp3')">Infância e Dificuldades</button>
    <button onclick="showContent('carreira', 'st3.gif', 'musica3.mp3')">Início da Carreira</button>
    <button onclick="showContent('conquistas', 'st4.gif', 'musica4.mp3')">Empreendedorismo e Conquistas</button>
    <button onclick="showContent('licoes', 'st5.gif', 'musica5.mp3')">Lições para Administração</button>
    <button onclick="showContent('conclusao', 'st6.jpg', 'musica6.mp3')">Conclusão</button>

    <div id="intro" class="content">
      <h2>Introdução</h2>
      <p>Neste trabalho, vamos conhecer a inspiradora história de Oprah Winfrey, uma mulher que superou a pobreza, os traumas da infância e os preconceitos sociais para se tornar uma das empresárias mais influentes do mundo.</p>
    </div>

    <div id="infancia" class="content">
      <h2>Infância e Dificuldades</h2>
      <ul>
        <li>Nascida em 1954 no Mississippi, em uma família muito pobre.</li>
        <li>Criada pela avó em condições precárias.</li>
        <li>Vítima de abusos na infância e gravidez precoce.</li>
        <li>Perdeu o bebê ainda recém-nascido.</li>
        <li>Manteve o foco nos estudos e acreditava em um futuro melhor.</li>
      </ul>
    </div>

    <div id="carreira" class="content">
      <h2>Início da Carreira</h2>
      <ul>
        <li>Começou no rádio com 17 anos.</li>
        <li>Se destacou na TV com seu carisma e empatia.</li>
        <li>Rompendo barreiras raciais, ganhou seu próprio programa.</li>
        <li>Estreia de <i>The Oprah Winfrey Show</i> em 1986.</li>
      </ul>
    </div>

    <div id="conquistas" class="content">
      <h2>Empreendedorismo e Conquistas</h2>
      <ul>
        <li>Fundou a Harpo Productions.</li>
        <li>Tornou-se a primeira mulher negra bilionária.</li>
        <li>Criou a Oprah Winfrey Network (OWN).</li>
        <li>Investiu em revistas, livros e causas sociais.</li>
        <li>Fundou escolas para meninas na África do Sul.</li>
      </ul>
    </div>

    <div id="licoes" class="content">
      <h2>Lições para a Administração</h2>
      <ul>
        <li><strong>Resiliência:</strong> transformou traumas em força.</li>
        <li><strong>Empatia:</strong> liderou com humanidade e conexão.</li>
        <li><strong>Marca pessoal:</strong> investiu em si mesma como negócio.</li>
        <li><strong>Visão estratégica:</strong> expandiu para várias mídias.</li>
      </ul>
    </div>

    <div id="conclusao" class="content">
      <h2>Conclusão</h2>
      <p>A trajetória de Oprah Winfrey mostra que é possível alcançar o sucesso mesmo em meio às maiores adversidades. Sua história é um verdadeiro exemplo de superação, liderança e visão empreendedora que inspira não apenas o mundo dos negócios, mas também todos que sonham em transformar suas vidas.</p>
    </div>
  </div>

  <audio id="audio" src="" preload="auto"></audio>

  <script>
    function showContent(id, gifPath, musicPath) {
      // Esconde todas as seções
      document.querySelectorAll('.content').forEach(section => section.style.display = 'none');

      // Mostra a seção selecionada
      document.getElementById(id).style.display = 'block';

      // Atualiza o GIF de fundo
      document.getElementById('gif').src = gifPath;

      // Toca a música correspondente
      const audio = document.getElementById('audio');
      audio.src = musicPath;
      audio.play();
    }
  </script>

</body>
</html>
