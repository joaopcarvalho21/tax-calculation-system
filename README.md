
## Sistema de Cálculo de Impostos

### Descrição

Este projeto é um programa Java que calcula os impostos de contribuintes, que podem ser classificados como **pessoas físicas** (indivíduos) ou **pessoas jurídicas** (empresas). O programa coleta informações como nome, renda anual e, dependendo do tipo de contribuinte, despesas médicas ou número de empregados, para calcular os impostos devidos com base nas regras específicas para cada categoria.

---

### Funcionalidades

1. **Cadastro de Contribuintes**:
   - O programa permite a entrada de um número `n` de contribuintes.
   - Para cada contribuinte, o programa coleta:
     - Tipo de contribuinte: **Indivíduo (i)** ou **Empresa (c)**.
     - Nome do contribuinte.
     - Renda anual.
     - Despesas médicas (somente para indivíduos).
     - Número de empregados (somente para empresas).

2. **Cálculo de Impostos**:
   - **Indivíduos**:
     - Se a renda anual for inferior a 20.000, a taxa de imposto será de 15%, com dedução de 50% sobre as despesas médicas.
     - Se a renda anual for igual ou superior a 20.000, a taxa de imposto será de 25%, com dedução de 50% sobre as despesas médicas.
   - **Empresas**:
     - Se o número de empregados for superior a 10, a taxa de imposto será de 14%.
     - Se o número de empregados for igual ou inferior a 10, a taxa de imposto será de 16%.

3. **Exibição dos Resultados**:
   - O programa exibe os impostos pagos por cada contribuinte.
   - Exibe o total de impostos pagos por todos os contribuintes.

---

### Como Executar

1. Clone ou baixe o projeto.
2. Compile e execute o código Java.
3. Insira o número de contribuintes.
4. Insira as informações de cada contribuinte conforme solicitado.
5. O programa calculará e exibirá os impostos devidos por cada um e o total de impostos.

---

### Estrutura do Projeto

O projeto contém três classes principais dentro do pacote `entities` e uma classe de execução no pacote `application`:

- **TaxPayer (Classe Abstrata)**: Classe base para representar um contribuinte, com métodos e atributos compartilhados, como nome e renda anual.
- **Individual**: Subclasse de `TaxPayer` que representa uma pessoa física. Calcula o imposto com base na renda e nas despesas médicas.
- **Company**: Subclasse de `TaxPayer` que representa uma empresa. Calcula o imposto com base na renda e no número de empregados.
- **Program**: Classe principal que realiza a interação com o usuário, coleta os dados e exibe os resultados.

---

### Exemplo de Uso

#### Exemplo 1:

Entrada:
```plaintext
Enter the number of tax payers: 2
Tax payer #1 data:
Individual or Company(i/c)? i
Name: John
Anual income: 15000
Health expenditures: 2000
Tax payer #2 data:
Individual or Company(i/c)? c
Name: SoftTech
Anual income: 400000
Number of employees: 25
```

Saída:
```plaintext
TAXES PAID: 
John: $1750.00
SoftTech: $56000.00

TOTAL TAXES: $57750.00
```

---

### Tecnologias Utilizadas

- **Java 17**
- **Scanner** para entrada de dados.
- Estrutura de controle de fluxo para manipulação de condições de cálculo.
- **Orientação a Objetos** (Herança e Polimorfismo) para estender as funcionalidades de cálculo de impostos.

---

## Tax Calculation System

### Description

This project is a Java program that calculates taxes for taxpayers, which can be classified as **individuals** or **companies**. The program collects information such as name, annual income, and depending on the type of taxpayer, medical expenses or number of employees, to calculate the taxes owed based on specific rules for each category.

---

### Features

1. **Taxpayer Registration**:
   - The program allows input for `n` taxpayers.
   - For each taxpayer, the program collects:
     - Type of taxpayer: **Individual (i)** or **Company (c)**.
     - Taxpayer's name.
     - Annual income.
     - Health expenditures (for individuals only).
     - Number of employees (for companies only).

2. **Tax Calculation**:
   - **Individuals**:
     - If annual income is less than 20,000, the tax rate is 15%, with a 50% deduction on health expenditures.
     - If annual income is 20,000 or more, the tax rate is 25%, with a 50% deduction on health expenditures.
   - **Companies**:
     - If the number of employees is more than 10, the tax rate is 14%.
     - If the number of employees is 10 or fewer, the tax rate is 16%.

3. **Displaying Results**:
   - The program displays the taxes paid by each taxpayer.
   - It also displays the total taxes paid by all taxpayers.

---

### How to Run

1. Clone or download the project.
2. Compile and run the Java code.
3. Enter the number of taxpayers.
4. Enter the required information for each taxpayer.
5. The program will calculate and display the taxes for each taxpayer and the total amount of taxes.

---

### Project Structure

The project contains three main classes within the `entities` package and one execution class in the `application` package:

- **TaxPayer (Abstract Class)**: A base class representing a taxpayer, with shared methods and attributes such as name and annual income.
- **Individual**: A subclass of `TaxPayer` representing an individual. It calculates taxes based on income and medical expenses.
- **Company**: A subclass of `TaxPayer` representing a company. It calculates taxes based on income and the number of employees.
- **Program**: The main class that handles user interaction, collects data, and displays the results.

---

### Example of Use

#### Example 1:

Input:
```plaintext
Enter the number of tax payers: 2
Tax payer #1 data:
Individual or Company(i/c)? i
Name: John
Anual income: 15000
Health expenditures: 2000
Tax payer #2 data:
Individual or Company(i/c)? c
Name: SoftTech
Anual income: 400000
Number of employees: 25
```

Output:
```plaintext
TAXES PAID: 
John: $1750.00
SoftTech: $56000.00

TOTAL TAXES: $57750.00
```

---

### Technologies Used

- **Java 17**
- **Scanner** for user input.
- Control flow structure for tax calculation conditions.
- **Object-Oriented Programming** (Inheritance and Polymorphism) to extend tax calculation functionalities.

---

