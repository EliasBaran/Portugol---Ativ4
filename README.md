# Portugol---Ativ4

1-Faça um programa que mostre o valor total da compra de todos os livros.

programa {
	funcao inicio() {
		
		real livro1, livro2, livro3, livro4, livro5, livro6, Total
		
		livro1 = 26.9
		livro2 = 34.1
		livro3 = 29.9
		livro4 = 26.9
		livro5 = 50.0
		livro6 = 26.9
		
		Total = livro1 + livro2 + livro3 + livro4 + livro5 + livro6 
		
		escreva ("o valor total é de ", Total, " reais")
		
	}
}



2. Faça um programa dado quatro variáveis que (4 notas bimestrais), mostre a média.

programa {
	funcao inicio() {
		
		real Pbi, Sbi, Tbi, Qbi, Media, Media2
		
		escreva ("qual foi a media do seu primeiro bimestre? ")
		leia (Pbi)
		
		escreva ("e a do segundo? ")
		leia (Sbi)
		
		escreva ("e a do terceiro? ")
		leia (Tbi)
		
		escreva ("e a do quarto? ")
		leia (Qbi)
		
		limpa()

		Media = Pbi + Sbi + Tbi + Qbi
		Media2 = Media /4

		escreva ("a sua média é de ", Media2)
		
	}
}



3-Escreva um programa que dados as variáveis chamadas mãe e filha, troque seus valores.

programa {
	funcao inicio() {
		
		cadeia mae = "Tess"
		cadeia filha = "Anna"
		cadeia troca
		
		troca = mae
		mae = filha
		filha = troca
		
		escreva (mae, filha)
		
		
	}
}



4. Faça um programa que converta metros para centímetros.

programa {
	funcao inicio() {
		
		real Metros, Centimetros
		
		escreva ("qual o valor em metros? ")
		leia (Metros)
		limpa()
		
		Centimetros = Metros * 100
		
		escreva ("o resultado é ", Centimetros, "cm")
	}
}



5. Faça um programa que peça o raio de um círculo, calcule e mostre sua área.

programa {
	funcao inicio() {
		
		real PI, R, A
		PI = 3.14
		
		escreva ("qual é o valor do raio? ")
		leia (R)
		limpa()
		
		
		A = PI * R * R
		escreva ("a área deste circulo mede ", A, "cm")
		
		
	}
}



6-Faça um algoritmo que dadas as medidas de comprimento e largura,
calcule:
a. A área do gramado.
b. O dobro da área.
c. O dobro da área em centímetros.

programa {
	funcao inicio() {
		
		inteiro Base, Altura, A, A2, A3
		
		escreva ("qual a medida da largura do maracanã? ")
		leia (Base)
		
		escreva ("qual a medida do comprimento do maracanã? ")
		leia (Altura)
		limpa()
		
		A = Base * Altura
		A2= A * 2
		A3 = A2 * 100
		
		escreva ("a área do maracanã é de ", A, "m \n o seu dobro é de ", A2, "m \n e em centímetros fica ", A3, "cm")
	
		
	}
}



7-Faça um programa que leia quanto dinheiro uma pessoa tem de economia em reais e em
seguida:
a. Escreva na tela quantos Dólares faltam para comprar um PS5.
b. Escreva na tela quantos Reais faltam para comprar um PS5.
c. Escreva na tela quantos livros Harry Potter e a Ordem da Fênix poderiam ser
comprados com o mesmo valor.

programa {
	funcao inicio() {
		
		real PS5, PS5d, Livros, Economia, EconomiaD
		
		escreva ("quanto dinheiro voçê economizou? ")
		leia (Economia)
		limpa()
		
		EconomiaD = Economia /5.34
		PS5d = 1300 - EconomiaD
		
		PS5 = 6947.33 - Economia
		
		Livros = 6947.33 /50
		
		se (Economia >= PS5) { escreva ("parabéns, voçê já pode comprar um ps5!")}
		
		senao {escreva ("faltam R$", PS5, " ou ", PS5d, " dolares para voçê comprar um ps5 \n com esse dinheiro voçê poderia comprar ", Livros, " do Harry Potter")}
	
	}
}



8. Faça um programa que leia um número inteiro qualquer e mostre na tela a sua tabuada.

programa {
	funcao inicio() {
		
		inteiro Num, contador, tabuada
		
		escreva ("fale um número: ")
		leia (Num)
		limpa()
		
		para (contador = 1; contador <= 10; contador++)
		{
		    tabuada = Num * contador
		  escreva (Num, " X ", contador, " = ", tabuada, "\n")
		}
		    
	}
}



9. Toda vez que um pescador traz um peso de peixes maior que o estabelecido pelo
regulamento de pesca do estado de Santa Catarina (50 quilos) deve pagar uma multa de R$
4,50 por quilo excedente.
a. Escreva um programa que leia a variável peso_de_peixes e calcule o excesso.
b. Grave em uma variável chamada excesso, a quantidade de quilos além do limite e
na variável multa o valor da multa que o pescador deverá pagar.
c. Escreva na tela os dados do programa com as mensagens adequadas (quantidade de
peixe pescado, multa a ser paga, etc)

programa {
	funcao inicio() {
		
		real Peso, Excesso, Multa
		
		escreva ("quantos quilos de peixe voçê pescou hoje? ")
		leia (Peso)
		limpa()
		
		Excesso = Peso - 50
		Multa = Excesso * 4.50
		
		se (Excesso <= 0) 
		{ 
		    escreva ("ok, tenha um bom dia")
		}
		
		senao 
		{ 
		    escreva ("voçê pescou mais quilos do que o permitido, por isso terá de pagra uma multa de R$", Multa)
		}
		    
		
	}
}
