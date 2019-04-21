## Notebooks: Avaliação de Empresas/Negócios, Obrigações e Riscos Financeiros

### Visualização Remota
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/ASaragga/Notebooks.jl/master)

As alterações efetuadas no Binder não são persistentes remotamente. Todavia, será possivel guardar localmente os Notebooks alterados num elevado número de formatos. 

### Instalação em Computador Local

Primeiro, necessitamos de instalar a linguagem de programação [Julia](https://julialang.org) (download v1.1). Alternativamente também podemos instalar [Julia Pro](https://juliacomputing.com/case-studies/), cujo site apresenta muitos exemplos interessantes de domínios onde foram desenvolvidas aplicações avançadas na linguagem Julia. 

Adicionalmente, também devemos instalar a aplicação [Jupyter](https://jupyter.org). Tal irá permitir interagir com a linguagem Julia, combinando código de programação, resultados calculados, texto formatado, símbolos matemáticos e multimédia num único documento. 

Passo 1 - Iniciamos Julia fazendo duplo-click no ícone. Irá aparecer uma janela com o prompt julia>

Passo 2 (apenas caso não tenhamos instalado Julia Pro) - No prompt julia> digitamos,
```julia
using Pkg; Pkg.add("IJulia")
```
para instalar o kernel de Jupyter para a linguagem Julia. Este passo apenas necessita de ser feito da primeira vez. 

Passo 3 - Para lançar a aplicação **Jupyter** no nosso browser (e.g. Google Chrome, Safari, Microsoft Edge) digitamos no prompt julia>
```julia
using IJulia; notebook()
```
Da primeira vez que corrermos `notebook()`, será pergundado se pretendemos instalar Jupyter, ao que iremos responder afirmativamente. 

Opcional - Por omissão, o **centro de controlo** será aberto na nossa diretoria pessoal. No entanto, numa primeira fase, sugiro antes abrir o **centro de controlo** numa diretoria única onde guardamos os notebooks e dados, fazendo
```julia
using IJulia; notebook(dir="diretoria_com_notebook_e_dados")
```
Exemplo: se guardámos o notebook ```2019abr.ipynb```e o ficheiro de dados ```2019abr.csv``` na directoria ```C:\Trabalhos```, então lançaremos **Jupyter** digitando,

```julia
using IJulia; notebook(dir="C:\Trabalhos")
```
