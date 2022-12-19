Fonte original do projeto: https://github.com/cedricp/ddt4all

#####
# Instruções de uso

Recomendado para uso no Linux ou Mac. Para Windows, existe o instalador que é infinitamente mais simples [fonte grupo (download lento)](https://mhhauto.com/Thread-DDT4All-5-5-0-base-07-2019-Super-program-for-Renault-ELM327-ELS327-ObdLink), [meu drive](https://drive.google.com/file/d/1u12uYUhWARUXyZI08esllqUXO83YdR6r/view?usp=share_link).

 - Instalar o Python 3.8
 - Baixar o [banco de dados Renault](https://drive.google.com/file/d/1-IvhnflMsdkE7-GiEXA_CBxIdiwB39vy/view?usp=share_link)
 - Adicionar o arquivo do banco de dados (ecu.zip) na pasta raiz.
 
 ### Para Mac, tive a necessidade de seguir alguns passos a mais. Caso alguém testar com Linux, e precisa também, me avise pelo grupo.
 #### Mac Intel

 - Executar os comandos (Mac intel):
  ```
  pip3 install PyQt5
  pip3 install PyQt5-sip
  pip3 install PyQtWebEngine
  ```

  - Abra o arquivo `options.py` em algum editor de texto. Para isso eu recomendo o [sublime](https://www.sublimetext.com/)
  - Edite a linha 51
  - Substitua o conteúdo por esse valor: t = gettext.translation(filename, 'locale', fallback=True)
  - Salve o arquivo
  
  Com o terminal aberto na pasta do aplicativo, execute o comando: `python3 ddt4all.py`

  #### Mac M1

  - Executar o terminal em modo Rosetta, para isso:
    - Ache o terminal pelo Finder
    - Clique com o botão direito em cima do ícone
    - Clique em "Get Info" ou "Mais informações", ou algo semelhante.
    - Habilite a opção de "Open using Rosetta" ou "Abrir usando Rosetta"
    - Abra o terminal
  - Executar os comandos (Mac M1):
  ```
  /usr/bin/python3 -m venv env
  source env/bin/activate
  pip install --upgrade pip
  pip install PyQt5
  pip install PyQt5-sip
  pip install PyQtWebEngine
  ```

  - Abra o arquivo `options.py` em algum editor de texto. Para isso eu recomendo o [sublime](https://www.sublimetext.com/)
  - Edite a linha 51
  - Substitua o conteúdo por esse valor: t = gettext.translation(filename, 'locale', fallback=True)
  - Salve o arquivo
  
  Com o terminal aberto na pasta do aplicativo, execute o comando: `python3 ddt4all.py`


