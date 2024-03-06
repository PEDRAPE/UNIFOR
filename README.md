# UNIFOR
**disciplina** raciocino logico alg
**prof** prof, Ricadardo Carubi
## lista 1
### exercicio 03
Represente, em fluxograma e pseudocódigo, um algoritmo para determinar se um número
inteiro e positivo é par ou impar.

#### fluxograma
```mermaid
flowchart TD
a([inicio])-->b{{digite um numero:}}
b-->c[/numero/]
c-->d{numero>0}
d--F-->e{{o numero deve ser positivo}}
d--V-->F[resto= numero % 2]
F-->g(resto == 0)
g--não-->h{{numero impar}}
g--sim-->i{{numero par}}
h-->j(fim)
i-->j
e-->j
```


``` 
ALGORITIMO verifica_par_impar
DECLARE numero, resto INTEIRO
ESCREVA "Digite um número:"
LEIA numero
SE numero > 0 ENTAO
	resto = numero % 2
	SE resto == 0 ENTAO
		ESCREVA "O numero é par"
	SENAO
		ESCREVA "o numero é impar"
SENÃO	
	ESCREVA "O numero deve sernpositivo"
FIM                                                      
```








# TAREFA DE RLA
## Primeira questão

 ```mermaid
 graph 
 a(inicio) --> b[digite o valor da nota1:]
 b --> c[digite o valor da nota2]
c --> d((calcule: nota1+nota2==SOMA))
d --> e{se: SOMA%2<7}
	e--sim-->f[[REPROVADO]]
	e--não -->g[[APROVADO]]
f-->h(FIM)
g-->h
 ```

```
ALGORITIMO_aprovado_ou_reprovado
DECLARE nota1, nota2, soma, media
ESCREVA "digite uma nota"
LEIA nota1
ESCREVA "digite a outra nota"
LEIA nota2
CALCULE nota1+nota2
LEIA soma
CALCULE soma%2
LEIA media
SE media<7 
	ENTAO 
	 ESCREVA "APROVADO"
	SENAO 
	 ESCREVA "REPROVADO"
FIM
```
















