youtube.com/watch?v=tthIRPzN61Y&list=PLV8UqTQmhTnFEu709oUyEfuq8J4Od-uIS&index=18&ab_channel=OnlineTutorials

/**
### CSS

1. `.container`: Define um recipiente que abrigará o slider e centraliza seu conteúdo.
   - `position: absolute;`: Define a posição absoluta do container.
   - `width: 100vw; height: 100vh;`: Define a largura e altura como 100% da largura e altura da tela do dispositivo.
   - `overflow: hidden;`: Oculta qualquer conteúdo que exceda as dimensões do container.
   - `display: flex; justify-content: center; align-items: center;`: Aplica um layout flexível para centralizar o conteúdo horizontalmente e verticalmente.

2. `.slider`: Estiliza o slider em si.
   - `position: absolute;`: Define a posição absoluta do slider dentro do container.
   - `inset: 80px 200px 80px 80px;`: Define os valores de deslocamento superior, direito, inferior e esquerdo do slider dentro do container.
   - `background: #ccc;`: Define o fundo do slider como cinza claro.
   - `border-radius: 20px;`: Aplica bordas arredondadas ao slider.

3. `.slides`: Estiliza cada slide dentro do slider.
   - `position: absolute;`: Define a posição absoluta dos slides dentro do slider.
   - `top: 50%; transform: translateY(-50%);`: Centraliza verticalmente os slides.
   - `width: 240px; height: 320px;`: Define as dimensões dos slides.
   - `background: var(--img);`: Define a imagem de fundo do slide (a variável `--img` é definida inline no HTML).
   - `background-size: cover; background-position: center;`: Configura o dimensionamento e a posição da imagem de fundo.
   - `transition: 0.5s;`: Adiciona uma transição suave para alterações de estilo.
   - `border-radius: 20px;`: Aplica bordas arredondadas aos slides.
   - `box-shadow: 0 25px 50px rgba(0,0,0,0.5);`: Adiciona uma sombra ao slide para dar profundidade.
   - `display: flex; justify-content: flex-start; align-items: flex-end;`: Alinha o conteúdo dos slides na parte inferior.

4. `.buttons`: Estiliza os botões de navegação do slider.
   - `position: absolute; bottom: 15px;`: Define a posição dos botões na parte inferior do container.
   - `display: flex; gap: 20px;`: Usa um layout flexível para os botões com um espaçamento de 20px entre eles.

5. `.buttons span`: Estiliza cada botão.
   - `position: relative; width: 50px; height: 50px;`: Define as dimensões e posição dos botões.
   - `background: #111;`: Define o fundo dos botões como preto.
   - `cursor: pointer;`: Mostra o cursor do mouse como um indicador de que os botões são clicáveis.
   - `border-radius: 50%;`: Aplica bordas arredondadas aos botões.

### HTML

- Dentro do `<body>`, há um `<div>` com a classe `.container`, que contém todo o conteúdo do slider e os botões de navegação.
  - Dentro deste `<div>`, há um `<div>` com a classe `.slider`, que contém uma série de slides.
  - Cada slide é representado por um `<div>` com a classe `.slides`, e cada um possui seu próprio conteúdo (título e parágrafo) dentro de uma `<div>` com a classe `.content`.
  - No final do documento, há um script JavaScript que implementa a funcionalidade de navegação do slider, permitindo avançar para o próximo slide ou voltar para o slide anterior ao clicar nos botões correspondentes.
**/