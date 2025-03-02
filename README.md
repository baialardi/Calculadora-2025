# Calculadora-2025
 Fundamentos do Git - EBAC - Profissão: Analista de Dados

# Como executar
* Clonar o repositório .sh para sua máquina local.
* Acesse o diretório para onde o repositório foi clonado.
* Dê permissão de execução ao script Bash: chmod +x calculadora.sh

 ## Comandos que utilizei
#!bin/bash
#Atividade Prática

def calculate():
    operation = input('''
Por favor insira a operaÃ§Ã£o matemÃ¡tica que gostaria de realizar:
+ para adiÃ§Ã£o
- para subtraÃ§Ã£o
* para multiplicaÃ§Ã£o
/ para divisÃ£o
''')

    number_1 = float(input('Insira o primeiro nÃºmero: '))
    number_2 = float(input('Insira o segundo nÃºmero: '))

    if operation == '+':
        print('{} + {} = '.format(number_1, number_2))
        print(number_1 + number_2)

    elif operation == '-':
        print('{} - {} = '.format(number_1, number_2))
        print(number_1 - number_2)

    elif operation == '*':
        print('{} * {} = '.format(number_1, number_2))
        print(number_1 * number_2)

    elif operation == '/':
        print('{} / {} = '.format(number_1, number_2))
        print(number_1 / number_2)

    else:
        print('Essa nÃ£o Ã© uma operaÃ§Ã£o vÃ¡lida, por favor tente novamente.')

    ## Add função para laço de repetição
    again()

def again():
    calc_again = input('''
Você gostaria de fazer um novo cÃ¡lculo?
Por favor digite S para SIM ou N para NÃO.
''')

    if calc_again.upper() == 'S':
        calculate()
    elif calc_again.upper() == 'N':
        print('See you later.')
    else:
        again()

calculate()

## Comandos em Linux

Item 3

analistamari@Mari:~/modulo1/python$ ls -l
total 12
-rwxr-xr-x 1 analistamari analistamari 1986 Feb 11 13:21 calculadora.sh
-rw-r--r-- 1 analistamari analistamari   66 Feb 11 10:38 nome.py
-rwxr-xr-x 1 analistamari analistamari  107 Feb 11 10:40 python_script.sh
analistamari@Mari:~/modulo1/python$ chmod u+rw calculadora.sh
analistamari@Mari:~/modulo1/python$ chmod go-w calculadora.sh


Item 4

analistamari@Mari:~/modulo1/python$ ls
calculadora.sh  nome.py  python_script.sh
analistamari@Mari:~/modulo1/python$ chmod +x calculadora.sh
analistamari@Mari:~/modulo1/python$ ls
calculadora.sh  nome.py  python_script.sh

Item 5

analistamari@Mari:~/modulo1$ cd /home/analistamari/modulo1/python
analistamari@Mari:~/modulo1/python$ ls
calculadora.sh  nome.py  python_script.sh
analistamari@Mari:~/modulo1/python$ python3 calculadora.sh

Por favor insira a operação matemática que gostaria de realizar:
+ para adição
- para subtração
* para multiplicação
/ para divisão

# Funcionalidades do código Python
* Solicita ao usuário dois números inteiros.
* Oferece quatro opções de operações matemáticas:
## Adição
## Subtração
## Multiplicação
## Divisão
* Exibe o resultado da operação selecionada.
Permite que o usuário execute novas operações continuamente.

