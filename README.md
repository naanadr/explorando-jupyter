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

### Instalando dependências

A unica dependência desse projeto é o `jupyter-lab`, para instalar ele, execute no terminal:

```bash 
pip install jupyterlab
```

ou 

```bash 
conta install -c conda-forge jupyterlab
```

Para abrir o `jupyter-lab` execute no terminal:

```bash 
jupyter-lab
```

Pronto, agora é só acessar no navegador a url [http://localhost:8888](http://localhost:8888)

## Utilizando Jupyter Notebooks com R

Eu não sou uma usuária frequente de R, mas pesquisando na internet encontrei esse [tutorial](https://richpauloo.github.io/2018-05-16-Installing-the-R-kernel-in-Jupyter-Lab/) que explica como criar notebooks R no Jupyter. Talvez ele possa te ajudar o/s