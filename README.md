# Como configurar/instalar/usar o `okular` no `Linux Ubuntu`

## Resumo

Neste documento estão contidos os principais comandos e configurações para configurar/instalar/usar o `okular` no `Linux Ubuntu`.

## _Abstract_

_This document contains the main commands and settings for configuring/installing/using the `okular` on `Linux Ubuntu`._

## Descrição [2]

### `okular`

O `Okular` é um visualizador de documentos de código aberto e altamente funcional, projetado principalmente para exibir documentos PDF e outros formatos de arquivo, como EPUB, DJVU, XPS, entre outros. Ele oferece uma variedade de recursos, incluindo navegação por página, zoom, anotações, marcação de texto e muito mais, tornando-o uma ferramenta versátil para visualização e interação com documentos digitais. Além disso, o `Okular` é altamente personalizável, permitindo que os usuários ajustem a interface e as configurações de acordo com suas preferências.

### `okular-extra-backends`

O `okular-extra-backends` é um pacote complementar do Okular que adiciona suporte a diversos formatos de documentos além dos já suportados pela instalação padrão. Ele fornece backends (módulos de leitura) para abrir e visualizar arquivos como `FictionBook` (`.fb2`), `Comic Book` (`.cbz` e `.cbr`), `Mobipocket` (`.mobi`), `EPUB`, `OpenDocument` (`.odt`, `.ods`, `.odp`), `Markdown`, `CHM`, `DjVu`, entre outros, dependendo da versão da distribuição e das bibliotecas disponíveis. Esse pacote é especialmente útil para usuários que utilizam o Okular como visualizador universal de documentos, permitindo centralizar a leitura de diferentes formatos em uma única aplicação, mantendo recursos como pesquisa de texto, anotações, marcadores, navegação por índice e modo de apresentação.


## 1. Como configurar/instalar/usar o `okular` no `Linux Ubuntu` [1][3]

Para configurar/instalar/usar o `okular` no `Linux Ubuntu`, você pode seguir estes passos:

1. Abra o `Terminal Emulator`. Você pode fazer isso pressionando:

    ```bash
    Ctrl + Alt + T
    ```

2. Certifique-se de que seu sistema esteja limpo e atualizado.

    2.1 Limpar o `cache` do gerenciador de pacotes `apt`. Especificamente, ele remove todos os arquivos de pacotes (`.deb`) baixados pelo `apt` e armazenados em `/var/cache/apt/archives/`. Digite o seguinte comando:
    ```bash
    sudo apt clean
    ```

    2.2 Remover pacotes `.deb` antigos ou duplicados do `cache` local. É útil para liberar espaço, pois remove apenas os pacotes que não podem mais ser baixados (ou seja, versões antigas de pacotes que foram atualizados). Digite o seguinte comando:
    ```bash
    sudo apt autoclean
    ```

    2.3 Remover pacotes que foram automaticamente instalados para satisfazer as dependências de outros pacotes e que não são mais necessários. Digite o seguinte comando:
    ```bash
    sudo apt autoremove -y
    ```

    2.4 Buscar as atualizações disponíveis para os pacotes que estão instalados em seu sistema. Digite o seguinte comando e pressione `Enter`:
    ```bash
    sudo apt update
    ```

    2.5 **Corrigir pacotes quebrados**: Isso atualizará a lista de pacotes disponíveis e tentará corrigir pacotes quebrados ou com dependências ausentes:
    ```bash
    sudo apt --fix-broken install
    ```

    2.6 Limpar o `cache` do gerenciador de pacotes `apt` novamente:
    ```bash
    sudo apt clean
    ```

    2.7 Para ver a lista de pacotes a serem atualizados, digite o seguinte comando e pressione `Enter`:
    ```bash
    sudo apt list --upgradable
    ```

    2.8 Realmente atualizar os pacotes instalados para as suas versões mais recentes, com base na última vez que você executou `sudo apt update`. Digite o seguinte comando e pressione `Enter`:
    ```bash
    sudo apt full-upgrade -y
    ```

Para instalar o `okular` no `Linux Ubuntu` através do `Terminal Emulator`, você pode seguir os seguintes passos:

1. **Abrir o `Terminal Emulator`:** Você pode abrir o `Terminal Emulator` pressionando:

    ```bash
    Ctrl + Alt + T
    ```

2. **Instalar o `okular`:** Digite o comando:

    ```bash
    sudo apt install okular -y
    ```

3. **Instalar o `okular-extra-backends`**: Para instalar o `okular-extra-backends` e permitir que o `okular` consiga ler outros
formatos de documentos, digite o comando:

    ```bash
    okular-extra-backends
    ```

### 1.1 Código completo para configurar/instalar/usar

Para configurar/instalar/usar o `okular` no `Linux Ubuntu` sem precisar digitar linha por linha, você pode seguir estas etapas:

1. Abra o `Terminal Emulator`. Você pode fazer isso pressionando:

    ```bash
    Ctrl + Alt + T
    ```

2. Digite o seguinte comando e pressione `Enter`:

    ```bash
    sudo apt clean
    sudo apt autoclean
    sudo apt autoremove -y
    sudo apt update
    sudo apt --fix-broken install
    sudo apt clean
    sudo apt list --upgradable
    sudo apt full-upgrade -y
    sudo apt install okular -y
    sudo apt install okular-extra-backends -y
    ```


## Referências

[1] OPENAI.
**Instalar o `okular` no `linux ubuntu` pelo `terminal emulator`.**
Disponível em: <https://chat.openai.com/c/a34dde21-da52-4dd3-853c-13861272bf34> (texto adaptado).
ChatGPT.
Acessado em: 20/03/2023 17:11.

[2] OPENAI.
**Vs code: editor popular.**
Disponível em: <https://chat.openai.com/c/b640a25d-f8e3-4922-8a3b-ed74a2657e42> (texto adaptado).
ChatGPT.
Acessado em: 20/03/2024 17:10.

