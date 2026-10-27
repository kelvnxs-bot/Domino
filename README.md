# Dominó Online

Dominó tradicional para jogar com um amigo pelo navegador: gere um link, mande para ele e pronto.
Tem chat com mensagens rápidas ("Calma aí", "Já volto"…). É **um único arquivo** (`index.html`), sem servidor
próprio, sem banco de dados e sem cadastro.

## Como jogar

1. Abra o site e clique em **Gerar link de convite**.
2. Copie o link e mande para seu amigo (WhatsApp, etc.).
3. Quando ele abrir, a partida começa. **Deixe sua página aberta**: o jogo roda no seu navegador.
4. Use o botão **💬 Chat** para conversar. No computador o chat fica fixo ao lado da mesa.

Recarregou a página ou caiu a internet? É só abrir o mesmo link de novo, no mesmo navegador: a partida, o placar
e as mensagens voltam e o amigo reconecta sozinho.

## Regras

- 28 peças (0–0 a 6–6), 7 para cada um, 14 no monte.
- 1ª rodada: começa quem tem a maior carroça e é obrigado a jogá-la (sem carroças, a peça de maior soma).
  Nas seguintes, começa quem venceu a anterior.
- A peça precisa ter o número de uma das pontas; se encaixar nas duas, você escolhe.
- Sem jogada: compra do monte (uma por vez). Monte vazio: passa a vez.
- Vence quem bater. Jogo trancado: vence quem tem menos pontos na mão; pontos iguais = empate.

## Publicar no GitHub e na Vercel

1. **GitHub Desktop**: *File → New repository* (ou *Add local repository* nesta pasta) → *Publish repository*.
2. **Vercel**: *Add New → Project* → importe o repositório → *Deploy*. Não precisa configurar nada:
   sem build, sem variáveis de ambiente.

Também funciona no GitHub Pages ou abrindo o arquivo por qualquer hospedagem estática (precisa ser `https`).

## Como funciona por dentro

- A conexão entre os dois navegadores é direta (WebRTC), usando a biblioteca **PeerJS** e o servidor público
  gratuito dela só para os dois "se encontrarem". As jogadas e mensagens vão direto de um navegador para o outro.
- Quem gera o link é o **anfitrião**: o baralho embaralhado fica no navegador dele, que confere toda jogada (vez,
  peça, ponta). O amigo recebe só a própria mão e a mesa — as peças do anfitrião e o monte não são enviados a ele.
- A partida e o chat ficam salvos no navegador do anfitrião (localStorage).

## Limitações (honestas)

- **Confiança entre amigos**: como o baralho fica no navegador do anfitrião, alguém com conhecimento técnico
  poderia espiar o monte pelo console do navegador dele. O convidado não consegue. Para um jogo à prova de
  trapaça, seria preciso um servidor (como a versão com Supabase).
- **O anfitrião precisa ficar com a página aberta**. Se fechar, o amigo vê "desconectado" até ele voltar.
- **Mesmo navegador**: a reconexão depende do navegador usado. Abrir o link em outro aparelho ou numa aba anônima
  conta como outra pessoa (e o jogo responde "Jogo cheio"). Para testar sozinho, use dois navegadores diferentes.
- **Servidor público do PeerJS**: é gratuito e sem garantia; se estiver fora do ar, o link não conecta. Algumas
  redes corporativas ou de celular muito restritas podem bloquear a conexão direta.
- O chat não é guardado em nenhum servidor: só existe nos dois navegadores (últimas 100 mensagens no anfitrião).
