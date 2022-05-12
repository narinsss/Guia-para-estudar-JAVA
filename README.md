# Guia-para-estudar-JAVA
Um modo que tenho que fixar os estudos é fazer anotações, destacando por importância, dificuldade entre outros adjetivos. Deixo aqui disponível e espero ajudar alguém assim.

## Estudos Java   ◾ ⚠ ✔ ↴ ⏬

#### Variáveis ↴

- char = ' 66 '  - aspas simples (apenas 1 caractere);
- String = '' exemplo'' - aspas duplas;
- Float = número com ponto flutuante (pouco usado);
- Int = número real;
- double = números decimais (mais utilizado);
- boolean = true or false (é possível citar outra variavel e condicionar);
- private algumaClasse nomeDoAtributo; = integrar atributos de outra classe;

#### Condicionais ↴


`If (condição 1) {`

`Sysout()`

`}else{`

`condição2`

`};`


- While = estrutura de repetição, significa 'enquanto'. 

  Exemplo:
  
`int i = 0;`

 `while (i <= 10){` 

`System.out.println(i);`

 `i++;` 

`};`

- For = estrutura de laço, escopo restrito

  Exemplo:
  
 `for(int i = 0; i <= 20; i++){`

 `System.out.println(i);` 

`};`

Diferença: While instancia de fora do escopo.

#### Operadores ↴

- ||  'pipe', 'barra vertical' = ou
- && = e
- == 
- != Diferente
- variável++ = +1
- variável += quando é var = var + var2;
- \n = quebra de linha



Dados e Funcionalidades (Ex. cpf, e validação do cpf)

#### ◾  Método ⏬

- Equivale a função


`void method(variable || argumento){`

`return` 

`condicionais`

`}`

- **Getters**  - método para os atributos privados que permite a utilização fora da classe-mãe, onde irá devolver os dados;

- **Setters** - método para os atributos privados que permite a modificação/alteração dos dados;

  #### **Método de formatar o número ↴** 

  `System.out.println(String.format("%04d", Classe.atributo++));`

  *O que significa cada parte:* 

  - **String.format**, usado para formatar o valor de objeto em cadeia de caracteres com base no formato que foi especificado;

  - **%d**, especificador para numero inteiro decimal;

  - **04**, numero deve conter quatro dígitos;

    

#### ◾  Construtor  ⏬ 

- **Parâmetros** - variável que deverá ser respondido nos objetos;
- **Herança** - Ao criar uma classe filha que irá herdar atributos da super class, é preciso gerar um construtor com os parâmetros que constam no construtor da super class;

#### ◾ Objetos ⏬ 

Instanciar uma classe, para criação de um **objeto**, exemplo:

`ClasseCadastro juliaObjetoQueEstaSendoCadastrado = new Cadastro(pode ou não ter parâmetros);`



#### ◾ Hierarquia/Herança(reutilização de código[extends]) ⏬

- Super class, Classe Mãe ou Base class;
- Classe filha = extends ou herda (A classe filha herda os atributos e métodos da classe mãe);

#### Composição ↴

- Para evitar repetição de métodos e atributos em todas as classes;
- Criando atributo com nome da ClassUtil, deve-se instancia-la no construtor das classes;

### **Polimorfismo** ↴

Chegar a um mesmo objeto do tipo ClasseTal, utilizando outra referência, pela classe mãe ou filha;

- @Override -> anotação do tipo sobrescrita, onde ao copiar um método da super.class, será necessário para checar se a assinatura está idêntica, caso não esteja o @Override não irá permitir a compilação do código, pois seria como um método novo;

- implements -> implementar uma interface à class;


#### ◾ Interface  ⏬

- Interface obriga as classes que a implementam, à utilizar todos os métodos;
- Uma interface não pode ter atributos, apenas métodos, e métodos sem corpo;
- As classes filhas que implementam uma interface, podem estender também a classe mãe;
- As classes podem implementar mais de uma interface;
- Todos os métodos devem ser abstratos;





#### Palavras-chaves

**this.atributo** = referencia atributo externos, ou seja, fora do método;

**return** = retorna valor da condição;

**static** = determina um único valor posto em um atributo de uma classe, para todos os objetos; utilizado mais para contadores, ou seja, verificar quantidade de objetos;

**super.atributo** = precisa acessar a classe mãe pra utilizar;

**abstract**= não permite que novos objetos sejam instanciados da classe, classes filhas apenas herdarão seus métodos e atributos;

- métodos abstract da classe mãe não devem ter corpo, pois serão desenvolvidos nas outras classes;

#### Modificadores de visibilidade

**private** = tornar atributos privados(encapsulamento), assim não poderão ser lidos ou modificados fora de sua classe mãe;

**protected** = visível apenas para as classes filhas;
