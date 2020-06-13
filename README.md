# Roteiro Live-Python

Referências: https://docs.python.org/pt-br/3/tutorial/, https://edisciplinas.usp.br/mod/folder/view.php?id=36176

## Introdução

### Instalação

### Linux

```bash
Geralmente o python vem instalado no Linux, por padrão
com a versão 2.7. 
Na live vamos usar a versão 3.7

Então verifique a versão do seu python com: 

ruan@shelby ~$ python3 --version ou python --version

Se não tiver instalado ou for menor 3.6 digite 
os seguintes comandos para instalação:

ruan@shelby ~$ sudo apt-get update
ruan@shelby ~$ sudo apt-get install python3.7
```

### Windows

```bash
Em geral os Windows mais antigos não vêm com python por padrão,
você pode instalar da seguinte forma:

Acessando o seguinte link:
https://www.python.org/ftp/python/3.8.3/python-3.8.3-amd64.exe

Caso houver algum erro, entre nesse site e faça download correto
para você:
https://www.python.org/downloads/windows/

Depois é so next, next, 

#Importante, quando aparecer a seguinte tela durante a instalação, 
#você deve clicar na opção : Add Python 3.8 to PATH

e só dar next next

```

![](https://raw.githubusercontent.com/ORuan/ORuan.github.io/master/Roteiro%20Live%20Python%20c1bba646130a4d368d8988654ede6f58/Untitled.png)

Módulos e formas de execução

```bash
python3 -m "module" for execute modules 
		   or
python3 -c "COMANDO/CÓDIGO"
```

### Bibliotecas

> Bibliotecas são conjuntos de funções criadas para resolver determinado problema

Qual a diferença entre uma biblioteca e um framework

Frameworks são conjunto de estruturas (modelos de projeto, funções, rotinas pré-definidas)

Fica mais fácil abstrair quando se compara com um códigos de programadores que já passaram pelos mesmo problema que você e estão tiveram a boa vontade de agrupar essas repetições e disponibilzar para os próximos. Ex: Django

- [ ]  Bibliotecas Importantes
    - sys
    - os
    - smtplib(Enviar email)
    - urllib.request (Acessar internet)

Conceitos básicos

Tipagem dinâmica

- Tipos principais
    - Int
    - Float

    - String
    - Tipos 'Complexos'
        - Dic
        - Array
        - Tuple

### Objects

"Formas de bolo"

```python
def cria_conta(numero, titular, saldo, limite):
    conta = {"numero": numero, "titular": titular, "saldo": saldo, "limite": limite}
    return conta
```

## Tratamento de dados

- Tá mas como eu deixo meu código de fato 'inteligente ?'

> Antes de prosseguir, é nessesário saber algumas coisas.
No Python não usamos " ; ", e as funções/estruturas de tratamento não são definidas com chaves;

### IF - ELSE (Estruras de decisão)

```python
color = 'blue'
if color === "blue":
    print('tu já sabe que é igual ne menó')
else:
    print('tu fez alguma cagada...')
```

### FOR

```python
i = [1,2,3,4,5,6]
for index in i:
   print(index)
   #espera-se que retorne:
   #1
   #2
   #3
   #4
   #5
   #6
#----------------------Usando Range()----------------

i = 0
for range(5):
    print(i)
    i = i+1
    

```

## Funções

São objetos de primeira classe no Python, como um objeto qualquer. 

### Tá, e o que isso significa?

Que podemos atribuir uma função a uma variável, podemos passar uma função como parâmetro para outra função, definir uma função dentro do escopo de outra, etc.

```python
def doble(number):
    return number*2
    #espera-se que retorne 4 se eu number for 2
```
