# explorando-jupyter
Uma viagem para conhecer a ferramenta - CODA.br 2022

Esse repositório contém o material utilizado no workshop "Explorando Jupyter: uma viagem para conhecer a ferramenta", ministrado no [CODA.br 2022](https://escoladedados.org/coda/coda2022/)

## Apresentação

A apresentação utilizada pode ser encontrada no [link](https://www.canva.com/design/DAFPI2kA414/7mT6sRCaxHgntnIPywMilA/view?utm_content=DAFPI2kA414&utm_campaign=designshare&utm_medium=link2&utm_source=sharebutton), ou no [PDF](slide_coda2022.pdf)

## Ambiente de desenvolvimento

Os experimentos aqui realizados ocorrem no **Python 3.10.6** para instalar e configurar o ambiente, realize os seguintes passos:

### Instalar o pyenv

O [pyenv](https://github.com/pyenv/pyenv) é uma ferramenta sensacional, que permite você instalar mais de uma versão do Python na sua máquina. 

Recomendo fortemente você instalar essa ferramenta o/ 

Caso você queira instalar ela, veja [essa página](https://github.com/pyenv/pyenv#installation). Mas se você estiver no Windows, veja [essa outra página](https://github.com/pyenv-win/pyenv-win#introduction).

> Para executar os experimentos aqui mostrados, não é obrigatório ter o pyenv instalado.

Depois de instalar o pyenv, vá para o terminal e faça:

```bash
pyenv install 3.10.6
cd explorando-jupyter
pyenv local 3.10.6
```

Nos comandos a cima, você instalou a versão `3.10.6` do python, entrou dentro da pasta `explorando-jupyter` e definiu que dentro dessa pasta a versão do Python que será utilizada é a `3.10.6`. 

### Criando um ambiente virtual

Quando desenvolvemos código em Python, geralmente criamos ambientes virtuais. Eles são como um ambiente fechado de desenvolvimento, onde tudo o que instalarmos nele, será apenas dentro dele. Isso nós permite ter ambiente de desenvolvimento separados para cada projeto que fazemos. Caso você queira saber mais sobre isso, assista [essa palestra](https://youtu.be/abTLJtSjclg) que eu fiz na Python Brasil 2020.

> Para executar os experimentos aqui mostrados, não é obrigatório criar um ambiente virtual.

Para criar um ambiente virtual, execute (dentro da pasta `explorando-jupyter`):

```bash 
python3 -m venv coda2022
```

Você só precisa criar o ambiente uma unica vez. Para saber se o ambiente foi criado, execute no terminal: 

```bash
ls
``` 

Você verá que foi criado uma pasta chamada `coda2022` \o/ 

Para ativar o ambiente virtual, execute: 

```bash
source coda2022/bin/activate
```

Pronto o/ 

Toda vez que você for trabalhar nesse projeto, execute esse comando no terminal. 

Para desativar o ambiente, execute:

```bash
deactivate
```

### Instalando dependências

> Caso você for utilizar ambientes virtuais: Instale as dependencias APENAS após ativar o ambiente virtual. 

Para instalar as dependências desse projeto, execute

```bash 
pip3 install -r requirements.txt
```

Esse comando irá instalar todas as dependências necessárias para atibar o `jupyterlab` e executar o notebook de exemplo.

Para ativar o jupyterlab, execute:

```bash
jupyter-lab
```

Se esse comando não funcionar, execute:

```bash
python3 -m jupyter-lab
```

Pronto, agora é só acessar no navegador a url [http://localhost:8888](http://localhost:8888)

## Utilizando Jupyter Notebooks com R

Eu não sou uma usuária frequente de R, mas pesquisando na internet encontrei esse [tutorial](https://richpauloo.github.io/2018-05-16-Installing-the-R-kernel-in-Jupyter-Lab/) que explica como criar notebooks R no Jupyter. Talvez ele possa te ajudar o/s
