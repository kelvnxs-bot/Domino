# Mesa de Jogos

Jogos para dois pelo celular ou computador: gere o número da sala, passe para um amigo e escolham no menu entre
**Dominó, Última!, Pontinhos, Jogo da Velha, Ligue 4 e Forca**. Tem chat com mensagens rápidas ("Calma aí", "Já volto"…),
que continua o mesmo em todos os jogos. O jogo inteiro é o `index.html`, sem servidor próprio, sem banco de
dados e sem cadastro.

**⚙️ Ajustes** (na tela inicial ou no menu): tema claro/escuro, som, cor da mesa (verde, azul, vinho, madeira,
grafite), peças do dominó (branca, marfim, preta) e pintas coloridas ou de uma cor só.

**🏆 Ranking** (no menu): junta todas as partidas de todos os jogos — você e cada adversário ordenados por vitórias,
mais uma tabela das suas partidas por jogo. Fica salvo no aparelho; dá para zerar (dois toques).

## Instalar como app

- **Pelo navegador (grátis, Android e iPhone):** abra o site e toque em **📲 Instalar app** na tela inicial
  (no iPhone: Safari → Compartilhar → *Adicionar à Tela de Início*). Abre em tela cheia, com ícone,
  e se atualiza sozinho quando o site é publicado.
- **App de verdade no iPhone (teste grátis de 7 dias pelo Xcode):** veja `app-iphone/INSTALAR-NO-IPHONE.md`.

No app, a tela não apaga durante a partida e o celular vibra quando chega a sua vez ou uma mensagem
(vibração só no Android; o iPhone não permite em sites).

## Como jogar

1. Abra o site, digite seu nome e toque em **Gerar número da sala**. Aparece um número de 4 dígitos (ex.: 4821).
2. Toque em **Mandar no WhatsApp** (ou **Copiar convite**): vai o número e o link.
3. Seu amigo digita o nome dele e o **número da sala** e toca em **Entrar na sala**.
   Pelo link, o número já vem preenchido (e se o nome dele já estiver salvo, entra direto).
   Os dois caem no menu: qualquer um escolhe o jogo e os dois entram juntos.
   **Deixe sua página aberta**: o jogo roda no seu navegador.
   - Número que não existe: aparece "Sala não encontrada".
   - Cada sala tem 2 jogadores. Se seu amigo trocar de celular, ele entra com o mesmo número (a vaga é liberada
     quando o aparelho anterior cai).
   - Várias salas funcionam ao mesmo tempo; se o número sorteado já estiver em uso, o site sorteia outro.
4. **Sair** volta os dois ao menu. A partida fica guardada: ao escolher o mesmo jogo de novo, ela continua.
   Cada jogo tem seu próprio placar.
5. No menu, **Fechar sala** (dois toques) encerra a sala e o número deixa de valer. Para o amigo, o botão é
   **Sair da sala**.
6. Use o botão **💬 Chat** para conversar. No computador o chat fica fixo ao lado da mesa.
7. **Série**: na faixa abaixo do topo, toque em *jogar uma série* e escolha melhor de 3, 5 ou 7. A faixa mostra
   o placar da série; quando alguém fecha, aparece o campeão e o botão vira **Revanche (nova série)**.
8. **Aviso na aba**: se você estiver em outra aba ou janela, o título pisca "🔔 Sua vez!" quando chegar a sua vez,
   e "💬 Nome: mensagem" quando chegar mensagem. Para de piscar quando você volta.

### Jogar sozinho

Na tela inicial, **🃏 Jogar sozinho** abre um menu com:

- **Dominó contra o Bot-Kelvin** — placar, séries e revanche funcionam igual. O Bot-Kelvin só usa o que um
  jogador de verdade enxerga: a própria mão, a mesa, quantas peças você tem e quando você comprou ou passou.
  Prefere bater, soltar peças pesadas e carroças cedo e deixar na mesa números que você não tem
  (vence cerca de 60% contra jogadores simples — dá para ganhar dele).
- **Paciência** (clássica, compra de 1 carta) — toque numa carta e ela vai sozinha para o lugar certo;
  se houver mais de um lugar possível, os destinos ficam marcados em verde e você toca no escolhido.
  Toque no monte para virar cartas. Tem **Desfazer**, **Nova partida** (pede confirmação) e **Terminar**,
  que sobe tudo para as fundações quando todas as cartas já estão viradas. Conta vitórias e partidas.

**Sair** volta ao menu; Sair no menu volta à tela inicial. As partidas ficam salvas (separadas das online).

Recarregou a página ou caiu a internet? Reconecta sozinho em poucos segundos, sem digitar o número de novo
(no mesmo navegador): a partida, o placar e as mensagens continuam.

## Regras do dominó

- 28 peças (0–0 a 6–6), 7 para cada um, 14 no monte.
- 1ª rodada: começa quem tem a maior carroça e é obrigado a jogá-la (sem carroças, a peça de maior soma).
  Nas seguintes, começa quem venceu a anterior.
- A peça precisa ter o número de uma das pontas; se encaixar nas duas, você escolhe.
  Dá para tocar na peça ou **arrastá-la até a ponta** da mesa (a ponta onde ela vai cair fica verde).
- Sem jogada: compra do monte (uma por vez) — as peças ficam espalhadas e o monte é embaralhado de novo a cada
  compra, então a escolha é sorte de verdade. Monte vazio: passa a vez.
- Vence quem bater. Jogo trancado: vence quem tem menos pontos na mão; pontos iguais = empate.

## Outros jogos

- **Última!** (jogo de cartas coloridas, para dois): 108 cartas, 7 para cada um. Jogue uma carta da mesma
  cor ou do mesmo número/símbolo; o Coringa vai sobre qualquer uma e você escolhe a cor.
  Com dois jogadores, **Pula** e **Inverte** fazem você jogar de novo; **+2** e **+4** fazem o outro comprar
  e você joga de novo (não acumulam). Sem jogada, compre 1 carta: se ela servir, pode jogá-la; senão a vez passa.
  Com 1 ou 2 cartas, aperte **Última!** — se ficar com 1 sem ter gritado, o outro pode apertar
  **"não gritou! (+2)"** e você compra 2. Vence a rodada quem zerar a mão.

- **Pontinhos** (jogo dos pontinhos): tabuleiro de 5×5 quadrados. Na sua vez, toque entre dois pontos vizinhos
  para riscar uma linha. Quem fecha o 4º lado de um quadrado ganha o ponto (o quadrado fica com a sua cor e
  inicial) e **joga de novo**. Quando todos os 25 quadrados forem fechados, vence quem tiver mais.
- **Jogo da Velha**: ✕ e ◯, quem começa alterna a cada partida.
- **Ligue 4**: toque numa coluna para soltar a ficha; vence quem alinhar 4 (linha, coluna ou diagonal).
- **Forca**: um escolhe a palavra (com dica opcional), o outro chuta letras — 6 erros completam a forca.
  Os papéis trocam a cada rodada. Acentos contam como a letra normal (É = E). No computador dá para usar o teclado.

## Publicar no GitHub e na Vercel

1. **GitHub Desktop**: *File → New repository* (ou *Add local repository* nesta pasta) → *Publish repository*.
2. **Vercel**: *Add New → Project* → importe o repositório → *Deploy*. Não precisa configurar nada:
   sem build, sem variáveis de ambiente.

Arquivos: `index.html` (o jogo), `manifest.webmanifest` e `sw.js` (para instalar como app), `icons/` (ícones),
`app-iphone/` (projeto do Xcode; o `.vercelignore` impede que ele vá para o site).

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
