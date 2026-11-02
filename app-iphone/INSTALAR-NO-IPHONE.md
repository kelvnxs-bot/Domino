# Mesa de Jogos no iPhone (teste grátis de 7 dias)

Este projeto instala a Mesa de Jogos como um app de verdade no seu iPhone, usando só o seu Apple ID —
sem pagar a conta de desenvolvedor da Apple. O app abre o site
`domino-online-seven.vercel.app`, então **toda atualização publicada no site aparece no app sozinha**,
sem reinstalar. Sem internet, ele abre uma cópia guardada (o modo sozinho funciona).

## Primeira vez (uns 20 minutos, mais o download do Xcode)

1. **Instale o Xcode** pela App Store do Mac (é grátis e grande, cerca de 10 GB). Abra uma vez e aceite os termos.
2. **Entre com seu Apple ID no Xcode:** menu *Xcode → Settings… → Accounts* → botão **+** → *Apple ID*.
3. **Abra o projeto:** dê dois cliques em `App/App.xcodeproj` (nesta pasta).
   Na primeira vez o Xcode baixa os componentes do Capacitor (barra de progresso no topo) — espere terminar.
4. **Assinatura:** na coluna da esquerda clique em **App** (ícone azul) → aba **Signing & Capabilities** →
   em *Team*, escolha **Seu Nome (Personal Team)**.
   - Se aparecer erro dizendo que o *Bundle Identifier* já está em uso, troque
     `com.kelvnxs.mesadejogos` por outro, por exemplo `com.kelvnxs.mesadejogos2`.
5. **Ligue o iPhone no Mac pelo cabo** e toque em *Confiar* no iPhone.
6. **Ative o Modo de Desenvolvedor no iPhone:** *Ajustes → Privacidade e Segurança → Modo de Desenvolvedor* →
   ligar → o iPhone reinicia → confirme *Ativar*.
   (A opção só aparece depois de ligar o iPhone no Mac com o Xcode aberto.)
7. **Escolha o iPhone** na barra do topo do Xcode (onde aparece o nome do aparelho) e clique no **▶ (Run)**.
8. **Confie no desenvolvedor no iPhone** (só na primeira vez): *Ajustes → Geral → VPN e Gerenciamento de
   Dispositivos* → seu Apple ID → *Confiar*. Depois abra o app **Mesa de Jogos**.

## Depois de 7 dias

Com o Apple ID grátis, a Apple só deixa o app funcionar por **7 dias**. Quando ele parar de abrir:
ligue o iPhone no Mac, abra `App/App.xcodeproj` e clique no **▶** de novo. Leva 1 minuto e não perde nada
(as partidas e o placar ficam no iPhone).

Limites do Apple ID grátis: até 3 apps seus instalados ao mesmo tempo, renovação a cada 7 dias.

## Se um dia quiser pagar (opcional)

Com a conta de desenvolvedor da Apple (paga, anual) o app passa a valer por 1 ano e dá para mandar para
amigos pelo TestFlight. Não é preciso para testar — e o site/app instalável pelo Safari continua grátis.

## Alternativa sem Xcode

No iPhone, abra o site no **Safari** → *Compartilhar* → **Adicionar à Tela de Início**. Fica com o mesmo ícone,
abre em tela cheia, não expira e não precisa de Mac. (A tela inicial do site tem um link **📲 Instalar app**
que mostra esse passo a passo.)
