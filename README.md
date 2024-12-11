# DesafioControleFluxo

## Descrição
Este repositório contém a solução para o desafio "Controle de Fluxo". O objetivo é praticar conceitos de controle de fluxo em Java, incluindo exceções personalizadas, laços de repetição e validação de dados.

O programa recebe dois números inteiros como parâmetros e realiza as seguintes operações:

- Se o segundo número for menor que o primeiro, lança uma exceção personalizada `ParametrosInvalidosException` com a mensagem: **"O segundo parâmetro deve ser maior que o primeiro"**.
- Caso contrário, realiza um laço de repetição para imprimir os números incrementados até atingir o intervalo entre os dois valores.

## Estrutura do Projeto

### Classes

1. **`ParametrosInvalidosException`**
   - Classe personalizada que herda de `Exception`.
   - Representa a validação de negócios para garantir que o segundo parâmetro seja maior que o primeiro.

2. **`Contador`**
   - Contém o método principal (`main`) para capturar os parâmetros do usuário.
   - Valida os parâmetros e chama o método `contar`.
   - Trata a exceção `ParametrosInvalidosException`.

3. **Método `contar`**
   - Realiza a validação e, caso os parâmetros sejam válidos, executa um laço `for` para imprimir os números incrementados.

### Fluxo do Programa
1. O usuário é solicitado a digitar dois números inteiros.
2. O programa valida se o segundo número é maior que o primeiro.
3. Caso a validação falhe, a exceção personalizada é lançada com a mensagem apropriada.
4. Caso a validação seja bem-sucedida, o programa imprime os números incrementados.

## Exemplo de Saída

### Entrada Válida
**Entrada:**
```
Digite o primeiro parâmetro:
5
Digite o segundo parâmetro:
10
```
**Saída:**
```
Imprimindo o número 1
Imprimindo o número 2
Imprimindo o número 3
Imprimindo o número 4
Imprimindo o número 5
```

### Entrada Inválida
**Entrada:**
```
Digite o primeiro parâmetro:
10
Digite o segundo parâmetro:
5
```
**Saída:**
```
O segundo parâmetro deve ser maior que o primeiro.
```

## Tecnologias Utilizadas
- Linguagem: Java 11+
- IDE recomendada: IntelliJ IDEA, Eclipse ou VS Code

## Como Executar
1. Clone o repositório:
   ```bash
   git clone https://github.com/seu-usuario/DesafioControleFluxo.git
   ```
2. Abra o projeto em sua IDE preferida.
3. Compile e execute a classe `Contador`.

## Melhorias Futuras
- Adicionar testes unitários para validar os comportamentos do método `contar`.
- Permitir que os parâmetros sejam passados como argumentos de linha de comando.
- Internacionalização da mensagem de erro para outros idiomas.

## Contribuições
Contribuições são bem-vindas! Por favor, abra uma _issue_ ou envie um _pull request_ com suas sugestões.

## Licença
Este projeto está sob a licença MIT. Consulte o arquivo `LICENSE` para mais informações.

