# Toca das Corujas
# Códigos Binários, Funções de Onda e Teoria do Orbital Molecular Inc.
# Unidade Barão Geraldo CX

Script de criação de uma remaster XTDC_2020

- Distro mais leve que encontrei foi a Xubuntu Core https://unit193.net/xubuntu/core/
- Antes usava Remastersys, PinguyBilder, etc, mas o Cubic se apresentou  mais rápido
- Uso o encurtador de URLs http://bit.do logado para poder modificar depois
- Ícones baseados no pacote Win2-7 https://www.gnome-look.org/p/1012465
- Fontes MS extraídas diretamente de instalações Win10
- Vários lançadores ocultos do menu do painel, permanecendo disponíveis em /usr/share/applications
- Configurações diversas via diretório /etc/skel extraídas e revisadas de outras instalações XTDC_2020


Alguns pontos sobre as funções

**xtdc_ppa**<br>
Aplica os ppas para termos as versões mais recentes de vários programas.<br>
Preferi fazer uma função que executasse a adição dos ppas por linha.<br>


**xtdc_pkg**<br>
Instala os programas escolhidos.<br>
Diferente da xtdc_ppa, aqui eu listei os programas por grupos em uma variável de uma linha.<br>
O rclone é instalado via script com curl, que é instalado antes de tudo.<br>

Principais aplicativos<br>
*Internet<br>
Google Chrome + Extensões<br>
Rclone Browser*<br>
     
Multimídia<br>
*SMPlayer<br>
Simplescreenrecorder*<br>
     
Office<br>
*Geany (editor de textos simples)<br>
Google Docs e Google Planilhas através de extensão do Chrome<br>
Evince PDF*<br>
     
Acessórios<br>
*Calculadora SpeedCrunch<br>
Atalhos para printscreen (Print Screen) - seleciona uma região na tela, salva a foto com a data e carrega para área de transferência.<br>
Atalhos para rascunhos (Ctrl+Alt+C) - salva o texto da área de transferência, renomeia com a data.*<br>

**xtdc_chrome**<br>
Instala o Chrome e algumas extensões.<br>
<br>
*Adblock Plus - bloqueador de anúncios grátis<br>
Os anúncios bloqueados para Youtube™<br>
Downloads<br>
Google Tradutor<br>
Configurações especiais para Youtube<br>
Planilhas<br>
Documentos<br>
Documentos OFFILNE<br>
Editor do Office*<br>

**xtdc_limpa_atalhos**<br>
Limpa as traduções dos atalhos.<br>
Esconde os que não estarão disponíveis para usuário via menu de aplicativos.<br>

**xtdc_atalhos**<br>
Cria os atalhos para os programas disponíveis para usuário via menu de aplicativos.<br>

**xtdc_limpa_pkg**<br>
Desinstala programas que não serão utilizados.<br>

**xtdc_exe**<br>
Cria um arquivo xtdc na pasta bin para algumas funções como o xtdc_printa e xtdc_rascunho.<br>

**gred**<br>
Função que faz o download via wget de uma url reduzida (bit.do) que aponta para o Google Drive.<br>

**xtdc_tema**<br>
Instala o pacote de ícones, tema, fontes ttf, painel, skel e programas próprios xtdc.<br>

**xtdc_lista_func**<br>
Lista as funções do script.<br>

**xtdc_2020_install**<br>
Roda todas as funções anteriores.<br>

Rodar o script de instalação online direto:<br><br>

**wget -qO xtdc_2020_install.sh https://raw.githubusercontent.com/Pinhalito/xtdc_2020/master/xtdc_2020_install.sh && source xtdc_2020_install.sh**
