RITMO AMOLED — PWA DE GANHOS A CADA 3 MINUTOS

ATUALIZAR O APP EXISTENTE PELO CELULAR
1. Baixe e extraia este ZIP.
2. Abra o mesmo repositório do GitHub onde está a versão anterior.
3. Envie os 6 arquivos desta versão para a raiz do repositório, substituindo os arquivos antigos com os mesmos nomes.
4. Confirme o commit.
5. Aguarde o GitHub Pages publicar a atualização.
6. Feche completamente o Ritmo no celular e abra novamente. Caso ainda apareça a versão antiga, feche o app, abra o endereço do GitHub Pages no Chrome e atualize a página; depois abra o app instalado novamente.

ARQUIVOS
- index.html: aplicativo completo
- manifest.json: configuração de instalação do PWA
- sw.js: cache offline e notificações
- icon-192.png e icon-512.png: ícones do aplicativo

O QUE MUDOU
- Tema escuro AMOLED com preto absoluto (#000000) em toda a interface.
- Ao começar ou continuar, a interface normal é substituída por uma tela preta em tela cheia, com cronômetro, tempo para o próximo ganho e controles discretos.
- O botão Pausar muda para Continuar quando a sessão está pausada.
- Parar sessão encerra o cronômetro, retorna à tela principal e gera a imagem de resumo.
- Botão do cadeado removido.
- Animações, sombras, gradientes, blur e efeitos visuais removidos.
- Fonte Inter mantida; sem internet, o sistema usa a fonte alternativa do celular.

RECURSOS MANTIDOS
- + R$ 2,00 por ciclo completo de 3 minutos ativos.
- Saldo salvo no celular e editável.
- Pausar preserva o tempo parcial do ciclo; Continuar retoma de onde parou.
- Notificação a cada ciclo concluído.
- Resumo em imagem ao parar, com ganhos, tempo ativo, ciclos e saldo atual.
- Wake Lock para tentar manter a tela ligada enquanto o cronômetro está em andamento.
- Instalação como PWA e cache offline.

OBSERVAÇÕES IMPORTANTES
- A contagem e as notificações funcionam melhor com o PWA aberto em primeiro plano e a tela ligada. O Android pode atrasar notificações se suspender o navegador ou aplicar economia de bateria.
- A tela AMOLED preta ajuda a economizar energia principalmente em telas OLED/AMOLED; o consumo do painel varia conforme brilho, área acesa e aparelho.
- O app tenta entrar em tela cheia ao começar. A disponibilidade desse recurso depende do navegador e do modo como o PWA foi instalado.
- O saldo fica salvo no armazenamento local do navegador. Evite limpar os dados do app/site se quiser preservá-lo.
