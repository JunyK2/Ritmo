RITMO AMOLED — CONTROLES PELO PLAYER DO ANDROID / SMARTWATCH

ATUALIZAR O APP EXISTENTE
1. Baixe e extraia o ZIP.
2. Abra o mesmo repositório do GitHub Pages.
3. Envie TODOS os arquivos para a raiz, substituindo os antigos.
4. Confirme o commit e aguarde a publicação do GitHub Pages.
5. Feche o Ritmo completamente. Abra o endereço do GitHub Pages no Chrome, atualize a página e depois abra o app instalado.

ARQUIVOS
- index.html: aplicativo completo
- manifest.json: configuração do PWA
- sw.js: cache offline e notificações (cache atualizado para substituir o áudio anterior)
- silence.wav: áudio digital totalmente silencioso de 15 segundos, em loop, para ativar os controles de mídia (o Chrome Android exige pelo menos 5 segundos)
- icon-192.png e icon-512.png: ícones

CONTROLES DO PLAYER (ANDROID / SMARTWATCH)
- Play: começa o cronômetro quando parado; retoma quando pausado.
- Pause: pausa o cronômetro.
- Próxima faixa (Next): para a sessão e gera a imagem do resumo.
- Faixa anterior (Previous): zera o saldo para R$ 0,00 sem apagar a contagem que estiver em andamento.
- Cada comando remoto envia uma notificação explicando a ação.
- Depois de parar ou zerar o saldo, o player permanece preparado para iniciar outra sessão, enquanto o navegador mantiver a sessão de mídia disponível.

BOTÕES FÍSICOS DE VOLUME E POWER — LIMITAÇÃO DO NAVEGADOR
Um site/PWA não tem permissão para capturar de forma confiável os botões físicos de volume ou identificar o botão Power no Android. Alguns dispositivos/navegadores podem entregar eventos de tecla de volume; o app tenta reconhecer esses eventos e, se forem entregues, alterna entre iniciar/retomar e pausar, notificando a ação. Na maioria dos celulares, porém, o Android consome as teclas de volume para ajustar o volume e não informa a tecla ao site.

O botão Power também não é identificável pelo site: apagar/bloquear a tela pode apenas ocultar ou suspender a página, e isso não permite distinguir Power de troca de aplicativo ou outra causa. Por isso, o app não envia uma notificação falsa dizendo que o Power foi pressionado.

COMO HABILITAR O PLAYER
1. Abra o PWA instalado e toque em Começar pelo menos uma vez, com o celular desbloqueado.
2. Permita as notificações.
3. O app inicia uma faixa WAV de 15 segundos, em loop e com silêncio digital absoluto, para registrar uma sessão de mídia no Android. O Chrome Android exige duração mínima de 5 segundos para mostrar o player de mídia. O arquivo não contém música ou fala audível.
4. Abra o player de mídia nas notificações/tela de bloqueio ou no smartwatch. Use Play/Pause, Próxima e Anterior.
5. Para receber os controles novamente após o Android encerrar a sessão, abra o Ritmo e toque em Começar uma vez.

RECURSOS MANTIDOS
- R$ 2,00 a cada 3 minutos completos de tempo ativo.
- Pausa preserva o tempo parcial do ciclo.
- Saldo editável e salvo em localStorage (mesma chave ritmo_balance da versão anterior).
- Notificação de cada ciclo e notificações dos comandos do player.
- Relatório em imagem ao parar.
- Tela AMOLED preta, Wake Lock, instalação PWA e cache offline.

OBSERVAÇÕES
- A exibição dos controles de mídia varia por marca, versão do Android e navegador. O navegador pode encerrar a sessão de mídia quando o sistema economiza bateria.
- O PWA precisa estar instalado/aberto inicialmente e receber uma primeira interação para iniciar o áudio silencioso; navegadores bloqueiam reprodução automática sem gesto do usuário.
- A contagem e notificações funcionam melhor com o PWA aberto em primeiro plano. O Android pode suspender timers/notificações em segundo plano.
- A imagem do relatório não bloqueia os comandos do player; um comando Play fecha o relatório e inicia/retoma a sessão.
- Não limpe os dados do site/app para preservar o saldo local.
