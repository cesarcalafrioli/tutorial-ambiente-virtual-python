# Tutorial - Ativando ambiente virtual python

Este tutorial se trata de utilizar o módulo venv para a ativação e desativação do ambiente virtual python tanto em sistemas operacionais linux quanto windows, a fim de evitar possíveis conflitos entres versões de um mesmo projeto e, consequentemente, dores de cabeça ao desenvolvedor.

A única diferença da ativação entre os dois ambientes é o comando em si. O linux utiliza o comando source para a ativação, enquanto no windows apenas executamos diretamente o script .bat.

## Ativando o venv

Navegue até a pasta do projeto no qual você deseja criar um ambiente virtual e dentro dela abra o terminal. Com o terminal aberto, rode o conjunto de comandos referentes ao que você deseja realizar.

### Instalando o módulo do ambiente virtual
   
No caso do linux, é necessário que o módulo do ambiente virtual esteja instalado.
   
   1. Atualize o apt
    ```
    sudo apt update
    ```
   2. Instale a venv
    ```
    sudo apt install python3.10-venv
    ```

### Criando um ambiente virtual

   1. Navegue até a pasta do projeto no qual você deseja criar um ambiente virtual e dentro dela abra o terminal
   2. Crie o ambiente virtual
    ```python3 -m venv nome_do_ambiente_virtual
    ```

Caso você não especifique um nome para o ambiente virtual, por padrão será "venv".

### Ativando o ambiente virtual

   1. Navegue até a pasta do projeto no qual você deseja criar um ambiente virtual e dentro dela abra o terminal
   2. Ative o ambiente virtual
    ```
    source nome_do_ambiente_virtual/bin/activate
    ```
       
      **OBS**: Caso esteja em um ambiente windows, use o comando abaixo:
      ```nome_do_ambiente_virtual\Scripts\Activate```


### Desativando o ambiente virtual

   1. Navegue até a pasta do projeto do qual você deseja desativar o ambiente virtual
   2. Desative o ambiente virtual
     ```
     deactivate
     ```

Pronto! ativando o venv, é possível a instalação das dependências sem que haja conflito futuros.

## Referências

https://www.alura.com.br/artigos/ambientes-virtuais-em-python

https://www.treinaweb.com.br/blog/criando-ambientes-virtuais-para-projetos-python-com-o-virtualenv

https://docs.python.org/pt-br/3/library/venv.html


