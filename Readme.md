![Badge Concluido](http://img.shields.io/static/v1?label=STATUS&message=%20CONCLUIDO&color=GREEN&style=for-the-badge)
# :abacus: Calculadora de IMC
<dl>
<dd>IMC é a sigla para índice de massa corpórea, parâmetro adotado pela Organização Mundial de Saúde para calcular o peso ideal de cada pessoa.</dd>
<dd>O índice é calculado da seguinte maneira: divide-se o peso do paciente pela sua altura elevada ao quadrado. Diz-se que o indivíduo tem peso normal quando o resultado do IMC está entre 18.5 e 24.9.</dd>
</dl>
	
## :weight_lifting_man: Veja a interpretação do IMC:

| IMC			          | CLASSIFICAÇÃO			| OBESIDADE (GRAU)|
|-------------------|:-----------------:|----------------:|
|MENOR QUE 18.5		  |  MAGREZA			    | 0|
|ENTRE 18.5 E 24.9	|  NORMAL				    | 0|
|ENTRE 25.0 E 29.9	|  SOBREPESO			  |	1|
|ENTRE 30.0 E 39.9		|  OBESIDADE			  |	2|
|MAIOR QUE 40.0			    |  OBESIDADE GRAVE	|	3|

O primeiro código tem como finalidade interagir com o usuário para que ele digite seus dados e a calculadora gere o resultado do IMC, depois a forma como ele é calculado e uma função que mostra a classificação do usuário referente a tabela de IMC.

:movie_camera:

<img src=".\Animação.gif" alt="Código funcionando" width="600px" heidth="400px">

1.	Entrada de dados:
````python
nome = input('Digite o seu nome: ')
peso = float(input('Digite o seu peso: '))
altura = float(input('Digite a sua altura: '))
imc = peso / (altura**2)
imc
````
2.	Calculo do IMC:
````python
imc = peso / altura ** 2)
````

3.	Função:
````python
def calculo_imc():
nome = input('Digite o seu nome: ')
peso = float(input('Digite o seu peso: '))
altura = float(input('Digite a sua altura: '))
imc = round(peso / (altura**2),2)
````

Para juntar textos com os dados de uma variável, podemos utilizar os **textos formatados**.
Basta utilizar um **f** antes das aspas do texto e colocar a variável dentro de **chaves**
````python
print(f"{nome} está com o IMC de {imc}!")
````


No final um código que vai gerar um arquivo em formato pdf, utilizando um template para receber os resultados da calculadora e classificação do usuário

````python
pdf_reports.write_report(template, "ficha_aluno.pdf", use_default_styling=False)
````

## :computer: Técnicas e Tecnologias utilizadas:
- Converter tipos de dados
- Juntar texto com váriaveis
- Estrutura condicional **if** - **elif**
	
	- Google Colaboratory

### :books:  Bibliotecas:
pdf_reports



