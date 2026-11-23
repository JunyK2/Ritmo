RITMO — PWA DE GANHOS A CADA 3 MINUTOS

ARQUIVOS
- index.html: aplicativo completo
- manifest.json: configuração para instalar como PWA
- sw.js: notificações e funcionamento offline
- icon-192.png e icon-512.png: ícones do aplicativo

COMO PUBLICAR PELO CELULAR
1. Baixe e extraia o arquivo ZIP.
2. Crie um repositório no GitHub.
3. Envie TODOS os arquivos extraídos diretamente para a raiz do repositório (não envie apenas o ZIP).
4. No repositório, abra Settings > Pages.
5. Em Build and deployment, escolha Deploy from a branch.
6. Selecione a branch main e a pasta /(root), depois toque em Save.
7. Abra o endereço publicado pelo GitHub Pages no Chrome do Android.
8. Aceite as notificações quando tocar em Começar. Para instalar, use o menu do Chrome > Instalar app / Adicionar à tela inicial.

COMO FUNCIONA
- Cada ciclo completo de 3 minutos em execução adiciona R$ 2,00 ao saldo.
- Pausar preserva o tempo parcial do ciclo; Continuar segue de onde parou.
- Parar encerra a sessão e mostra uma imagem com ganhos, tempo ativo, ciclos e saldo.
- Toque em Editar saldo para definir o valor inicial ou corrigir o saldo.
- Toque no cadeado para bloquear os controles. Toque duas vezes no cadeado para desbloquear.
- O tema claro/escuro acompanha a configuração do celular.

IMPORTANTE SOBRE AS NOTIFICAÇÕES
Mantenha o PWA aberto em primeiro plano para os avisos saírem nos horários previstos. O app tenta impedir que a tela apague usando o recurso Wake Lock; permita essa função pelo navegador, se solicitado. O Android pode limitar timers/notificações quando o app fica em segundo plano, o aparelho bloqueia a tela ou o sistema economiza bateria. O saldo é calculado pelo tempo real decorrido quando o app está ativo, mas o aviso pode chegar atrasado se o sistema suspender a página.

A fonte Inter é carregada do Google Fonts quando há internet; se estiver offline, será usada uma fonte semelhante do sistema.
