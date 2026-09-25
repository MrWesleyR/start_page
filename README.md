# Start Page 

>Uma página incial para navegadores de internet com auto complete sem AI

<img src="img/startpage.png" alt="Imargem do Projeto StartPage" width="800" />


### Fucionalidades

1. Links favoritos.
2. Direcionamento para sites como youtube, github.
3. Fazer pesquisas em buscadores alternativos.
4. Autocomplete.
5. Abertura de links amigaveis, complexos e locais na barra de pesquisa.

#### Como utilizar 

``` bash

    # Para rodar em localhost o servidor node usando seu usuário sem root.
    pacman -S setcap 

    sudo setcap 'cap_net_bind_service=+ep' /usr/bin/node

    git pull https://github.com/MrWesleyR/startpage 

    cd startpage
    
    npm install
    
    node server 

```
### Com picom

``` json
Cores em .cache/wal/color.json

{
    "checksum": "989fe7f46470466cb44b08115bb7b1ab",
    "wallpaper": "/home/user/.wall/bg1.png",
    "alpha": "100",

    "special": {
        "background": "#1c1c1c",
        "foreground": "#c6c6c6",
        "cursor": "#c6c6c6"
    },
    "colors": {
        "color0": "#1c1c1c",
        "color1": "#4C4C4C",
        "color2": "#515151",
        "color3": "#555555",
        "color4": "#595959",
        "color5": "#5C5C5C",
        "color6": "#606060",
        "color7": "#c6c6c6",
        "color8": "#756060",
        "color9": "#4C4C4C",
        "color10": "#515151",
        "color11": "#555555",
        "color12": "#595959",
        "color13": "#5C5C5C",
        "color14": "#606060",
        "color15": "#c6c6c6"
    }
}

Serão resposavel pela mudança da coloração página ao trocar de wallpaper.

```

#### Como pequisar 

No momento e reconhecido os buscadores:

    - DuckDuckDuckGo
    - Google
    - StartPage
    - LibreY

Ao fazer uma pesquisa simples por padrão sera chamado o DuckDuckGo,
caso queira fazer pesquisas em outros buscadores digite o nome do buscador
na barra de pesquisa, siga os exemplos abaixo:

* DuckDuckGO -  du sua pesquisa aqui
* Google - go sua pesquisa aqui
* LibreY - ly sua pesquisa aqui
* StartPage - sp sua pesquisa aqui

Caso queira adicionar outros buscadores 
edite o arquivo [opener.js](public/home/js/miniEngine/opener.js#L83) .

Para mais direcionamentos de instâncias
edite o arquivo [opener.js](public/home/js/miniEngine/opener.js#L7) .

Para alias de serviços 
edite o arquivo [opener.js](public/home/js/miniEngine/opener.js#L27) .


# Picom 

Definição: Um compositor leve para X11
Source: https://github.com/yshui/picom

> [!WARNING]
> A página não foi hospedada remotamente porque precisa acessar o arquivo config.json para obter as cores do Picom. Embora fosse >possível desenvolver uma extensão para essa finalidade, isso não foi considerado necessário, uma vez que o projeto contempla apenas essa página.
>Por questões de segurança implementadas pelo próprio navegador, é necessário realizar o deploy do servidor. Seria possível contornar  essa limitação utilizando o Zen Browser; no entanto, a página funcionaria exclusivamente nesse navegador.

> [!NOTE]
> Em atualizações futuras, pretendo tornar a página mais intuitiva e fácil de usar, além de adicionar suporte a recursos dos temas mobile Material e implementar outras funcionalidades. 
