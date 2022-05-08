# FIBONACCI EXERCISE

#### [1] - Do the Fibonacci sequence a determined numbers of times
```python
def sequence():
  n1,n2 = 0,1
  acc = 0

  num=int(input("Informe quantos numeros de fibonacci voce deseja\n"))
  if num <=0:
      print("Entre com numeros acima de 0")
  elif num == 1:
      print("Sequencia:\n0")
  else:
      for i in range(num):         
          print(n1)
          fib = n1 + n2
          n1 = n2
          n2 = fib
```

#### [2] - Code verify if the informed number are in fibonacci sequence
```python
def verify():
import math

    num=int(input("Entre com um numero inteiro para verificar\n"))
    x1 = 5*num*num+4
    x2 = 5*num*num-4 

    if (math.ceil(math.sqrt(x1))== math.floor(math.sqrt(x1))):
        print(f"{num} faz parte da sequencia de fibonacci")
        
    elif (math.ceil(math.sqrt(x2))== math.floor(math.sqrt(x2))):
        print(f"{num} faz parte da sequencia de fibonacci")
        
    else:
        print(f"O {num} nao faz parte da sequencia de fibonacci")
        
```
#### Print 
```python
while True:
    op=int(input("[1] Sequencia fibonacci N vezes\n[2] Verificar se o numero é um numero de fibonacci\n[3] Sair\n"))

    if op == 1:
        sequence()
    if op == 2:
        verify()
    if op == 3:
        break
    
    while op <1 or op >3:
        print("Opção não reconhecida")
        op=int(input("[1] Sequencia fibonacci N vezes\n[2] Verificar se o numero é um numero de fibonacci\n[3] Sair\n"))

```
