
# O que é R?

###  Em uma tradução literal e seguindo o próprio site do [R Project](https://www.r-project.org/about.html "R Project") o R é uma linguagem e ambiente para computação estatística e gráficos.

---

#### Atribuição

---

Sinal usado para atribuição em R <-
`x<-4`
Então x recebe o valor 4

#### Vetores

---

 Em R, você cria um vetor com a função de combinação c (). Você coloca os elementos vetoriais separados por uma vírgula entre os parênteses. Por exemplo:

jogador<-(“Jonh”, “poker player”)
propriedades(jogador)<-(“Nome”,”Profissao”)
“If you want to become a good statistician, you have to become lazy. (If you are already lazy, chances are high you are one of those exceptional, natural-born statistical talents.)”


Como são realizadas as somas em R
É importante saber que se você soma um vetor em R, você irá fazer as somas de acordo com a ordem dos elementos, isto é, o primeiro elemento do primeiro vetor será somado com o primeiro elemento do segundo vetor.

c(1, 2, 3) + c(4, 5, 6)
c(1 + 4, 2 + 5, 3 + 6)
c(5, 7, 9)

Você também pode fazer soma com variáveis que representam os vetores:
a <- c(1, 2, 3) 
b <- c(4, 5, 6)
c <- a + b
A função sum() realiza a s,a de todos os elementos do vetor, logo se você fizer

sum(a)
a
O resultado será 6

Como são realizadas as seleções de elementos em R

 colchetes [ ] servem para delimitar o espaço do intervalo dos elementos que serão selecionados no vetor.

Selection by comparison - Step 1
É possível realizar comparações mesmo na atribuição
# Which days did you make money on poker?
> selection_vector <- poker_vector[c("Monday", "Tuesday", "Wednesday", "Thursday", "Friday")] > 0
> 
> # Print out selection_vector
> selection_vector
   Monday   Tuesday Wednesday  Thursday    Friday 
     TRUE     FALSE      TRUE     FALSE      TRUE

Selection by comparison - Step 2
# Which days did you make money on roulette?
> selection_vector <- roulette_vector > 0
> 
> # Select from roulette_vector these days
> roulette_winning_days <- roulette_vector[selection_vector]



04/07

What's a matrix?
> # Construct a matrix with 3 rows that contain the numbers 1 up to 9
> matrix(1:9, byrow = TRUE, nrow = 3)
     [,1] [,2] [,3]
[1,]    1    2    3
[2,]    4    5    6
[3,]    7    8    9
> 

Analyze matrices, you shall

box_office <- c(new_hope, empire_strikes, return_jedi)
> 
> # Construct star_wars_matrix
> star_wars_matrix <- matrix(box_office, byrow = TRUE, nrow = 3)
> # Box office Star Wars (in millions!)
> new_hope <- c(460.998, 314.4)
> empire_strikes <- c(290.475, 247.900)
> return_jedi <- c(309.306, 165.8)
> 
> # Create box_office
> box_office <- c(new_hope, empire_strikes, return_jedi)
> 
> # Construct star_wars_matrix
> star_wars_matrix <- matrix(box_office, byrow = TRUE, nrow = 3)
> 











> As anotações foram baseadas nesse curso [aqui](https://www.udemy.com/aprenda-markdown/). do [Roberto Achar](https://twitter.com/RobertoAchar) e adaptado da postagem da [Leticia](https://github.com/leticiadasilva/notas-de-aula)
