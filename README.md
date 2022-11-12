# Makefile

## Estrutura
~~~make
Alvo:   Dependência
    Comando
~~~

## 
~~~make
all: mensagem1
    @echo "Olá Mundo!"

mensagem1:
    @echo "Sou a mensagem 1"

mensagem2:
    @echo "Sou a mensagem 2"
~~~

~~~bash
make -n
~~~

Retorna os comandos que vão ser executados, sem executá-los.

~~~bash
make
~~~

Nesse caso o all tem a dependência mensagem1, então ele executa primeiro  
mensagem1 e depois o que está dentro de all.

~~~bash
make mensagem2
~~~

Só será exibido o que está dentro de mensagem2

~~~bash
make mensagem1
~~~

Só será exibido o que está dentro de mensagem1

## @

Por padrão o é mostrado o comando que vai ser executado e depois executa o comando.

Com o @ ele não mostra o que vai ser executado, somente executa.
