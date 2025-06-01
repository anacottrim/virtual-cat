# Boas Vindas ao projeto do Gatinho Virtual

<img src = "Imagens/tela.jpeg">

# O que é este projeto?

O projeto do Gato Virtual é inspirado no Tamagochi, e é composto de duas páginas web. Na primeira, você dá um nome para o gato, e na segunda página tem as interações com ele.
A segunda tela possui 5 botões de interação com o gato além de um chat, onde é possível conversar com o gato.
Cada botão de interação conta com uma reação do gato à atividade realizada, representada por um emoji. As interações disponíveis são:

- Alimentar - selecione um alimento para dar ao gato;
- Dar bebida - selecione uma bebida para dar ao gato;
- Brincar - selecione um brinquedo para o gato;
- Fazer carinho - faça um carinho ruim, mais ou menos, bom ou perfeito no gato;
- Acordar - acorde o gato se ele estiver dormindo, ou o coloque para dormir se ele estiver acordado. Lembrando que as outras interações ficam indisponíveis quando o gato está acordado.

# Como utilizar este projeto?

Você pode acessar este projeto [clicando aqui](https://lelepg.github.io/Virtual-Cat/index.html).
De maneira alternativa você também pode fazer o download deste repositório cloando-o ou baixando em formato _.zip_.
Caso opte por baixar em _.zip_, descompacte o arquivo baixado e abra o arquivo **index.html** clicando duas vezes sobre ele. Isso abrirá a página inicial, onde o nome do gato deve ser escolhida. Depois de nomear o gato, clique em iniciar para ter acesso à página de interações.

### Tecnologias utilizadas

- HTML;
- CSS;
- Javascript.

### Links externos:

- [Emojis](https://unicode.org/emoji/charts/full-emoji-list.html)
- [Imagem original utilizada para o gato](https://fi.pinterest.com/pin/863706034772772147/)

- # 🐳 Dockerização do Projeto (Etapa do Projeto Individual)

Este repositório foi **dockerizado** com o objetivo de facilitar sua execução em qualquer máquina que possua o Docker instalado.

Abaixo, segue o passo a passo detalhado para rodar o projeto via Docker.



## ⚙️ Como rodar este projeto com Docker

### 1. Clone este repositório:

git clone https://github.com/anacottrim/virtual-cat.git

cd virtual-cat

### 2. Crie a imagem Docker:

docker build -t virtual-cat .

Esse comando cria uma imagem Docker com o nome virtual-cat a partir do Dockerfile presente no projeto.

### 3. Rode o container:
   
docker run -d -p 8080:80 virtual-cat

Este comando executa o container em segundo plano (-d) e faz o mapeamento da porta 80 do container para a porta 8080 da sua máquina local.

### 4. Acesse o site no navegador:
Se você está rodando diretamente no Linux ou WSL:
Abra o navegador e acesse:

http://localhost:8080

Se você estiver usando uma máquina virtual (como no VirtualBox):
Descubra o IP da sua VM:
ip a
Procure por uma linha como inet 192.168.x.x.
Depois, no navegador da sua máquina real, acesse:

http://192.168.x.x:8080

📥 Alternativa: usar a imagem do Docker Hub
Se preferir, você pode usar diretamente a imagem que subi no Docker Hub:

docker pull anacotrim/virtual-cat

docker run -d -p 8080:80 anacotrim/virtual-cat

✅ Resultado esperado
Se tudo estiver certo, você verá a página inicial do Gato Virtual no navegador, podendo:

Dar nome ao seu gato;

Interagir com ele;

Usar todos os recursos visuais e de chat da aplicação.

📌 Observações
O projeto foi mantido como originalmente desenvolvido, sem alterações no código HTML/CSS/JS.

A Dockerização foi feita apenas para facilitar a execução da aplicação.

Esta atividade faz parte de um projeto individual com entrega obrigatória.

🛠️ Feito por @anacotrim – Junho/2025


