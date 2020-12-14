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

###xtdc_ppa

Aplica os ppas para termos as versões mais recentes de vários programas
Preferi fazer uma função que executasse a adição dos ppas por linha


###xtdc_pkg

Instala os programas escolhidos
Diferente da xtdc_ppa, aqui eu listei os programas por grupos em uma variável de uma linha
O rclone é instalado via script com curl, que é instalado antes de tudo
Principais aplicativos

Internet - 
Google Chrome + Extensões
Rclone Browser
     
Multimídia - 
SMPlayer
Simplescreenrecorder
     
Office - 
Geany (editor de textos simples)
Google Docs e Google Planilhas através de extensão do Chrome
Evince PDF
     
Acessórios - 
Calculadora SpeedCrunch
Atalhos para printscreen (Print Screen) - seleciona uma região na tela, salva a foto com a data e carrega para área de transferência
Atalhos para rascunhos (Ctrl+Alt+C) - salva o texto da área de transferência, renomeia com a data


###xtdc_chrome

Instala o Chrome e algumas extensões
Adblock Plus - bloqueador de anúncios grátis
Os anúncios bloqueados para Youtube™
Downloads
Google Tradutor
Configurações especiais para Youtube
Planilhas
Documentos
Documentos OFFILNE
Editor do Office


###xtdc_limpa_atalhos

Limpa as traduções dos atalhos
Esconde os que não estarão disponíveis para usuário via menu de aplicativos


###xtdc_atalhos

Cria os atalhos para os programas disponíveis para usuário via menu de aplicativos


###xtdc_limpa_pkg

Desinstala programas que não serão utilizados

###xtdc_exe

Cria um arquivo xtdc na pasta bin para algumas funções como o xtdc_printa e xtdc_rascunho

###gred

Função que faz o download via wget de uma url reduzida (bit.do) que aponta para o Google Drive


###xtdc_tema

Instala o pacote de ícones, tema, fontes ttf, painel, skel e programas próprios xtdc


###xtdc_lista_func

Lista as funções do script


###xtdc_2020_install

Roda todas as funções anteriores


Rodar o script de instalação online direto:

wget -qO xtdc_2020_install.sh https://raw.githubusercontent.com/Pinhalito/xtdc_2020/master/xtdc_2020_install.sh && source xtdc_2020_install.sh
