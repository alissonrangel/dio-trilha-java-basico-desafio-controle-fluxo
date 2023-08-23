# dio-trilha-java-basico-desafio-controle-fluxo
## Repositório para o desafio Controle de Fluxo do Bootcamp de Java da DIO/Santander 2023

#### DIO - Trilha Java Básico
- [Trilha Java Básico](https://github.com/digitalinnovationone/trilha-java-basico)

#### Autor do Desafio
- [Gleyson Sampaio](https://github.com/glysns)

## Controle de Fluxo - Desafio

Vamos exercitar todo o conteúdo apresentado no módulo de Controle de Fluxo codificando o seguinte cenário.

O sistema deverá receber dois parâmetros via terminal que representarão dois números inteiros, com estes dois números você deverá obter a quantidade de interações (for) e realizar a impressão no console (System.out.print) dos números incrementados, exemplo:

* Se você passar os números 12 e 30, logo teremos uma interação (for) com 18 ocorrências para imprimir os números, exemplo: `"Imprimindo o número 1"`, `"Imprimindo o número 2"` e assim por diante.
* Se o primeiro parâmetro for MAIOR que o segundo parâmetro, você deverá lançar a exceção customizada chamada de `ParametrosInvalidosException` com a segunda mensagem: "O segundo parâmetro deve ser maior que o primeiro"   


1. Crie o projeto `DesafioControleFluxo`
2. Dentro do projeto, crie a classe `Contador.java` para realizar toda a codificação do nosso programa.
3. Dentro do projeto, crie a classe `ParametrosInvalidosException` que representará a exceção de negócio no sistema. 

Abaixo temos um trecho de código no qual você poderá seguir alterando as partes que contenham `??`

```java
public class Contador {
	public static void main(String[] args) {
		Scanner terminal = new Scanner(System.in);
		System.out.println("Digite o primeiro parâmetro");
		int parametroUm = terminal.??;
		System.out.println("Digite o segundo parâmetro");
		int parametroDois = terminal.??;
		
		try {
			//chamando o método contendo a lógica de contagem
			contar(parametroUm, parametroDois);
		
		}catch (? exception) {
			//imprimir a mensagem: O segundo parâmetro deve ser maior que o primeiro
		}
		
	}
	static void contar(int parametroUm, int parametroDois ) throws ParametrosInvalidosException {
		//validar se parametroUm é MAIOR que parametroDois e lançar a exceção
		
		int contagem = parametroDois - parametroUm;
		//realizar o for para imprimir os números com base na variável contagem
	}
}
```

### Aluno: Alisson Rangel [@alissonrangel](https://github.com/alissonrangel)

### Decisões de projeto
- java version "20.0.2" 2023-07-18, pois é a versão mais atual do Java;
- Projeto desenvolvido no vscode; 
- Uso da classe Scanner como pedido no desafio, optei por usar o método nextInt() da classe Scanner, pois vou capturar valores numéricos inteiros pelo teclado;
- Criação de uma Exceção customizada, na sua criação optei apenas por extendê-la de Exception por ser uma exceção checada;
```
public class ParametrosInvalidosException extends Exception{
}
```
- Uso da estrutura de repetição for para impressão dos números como pedido no desafio.
