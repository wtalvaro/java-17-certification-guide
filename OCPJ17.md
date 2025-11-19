### **Curso: Java SE 17 Developer Certification Prep**

#### **Módulo 1: Introdução ao Java e Fundamentos**

- **Conteúdo**:
  - Visão geral do ecossistema Java
  - Estrutura de classes e objetos
  - Membros de instância e estáticos
  - Herança e agregação
  - Compilação e execução de programas Java
- **Exemplo Prático**: Escrever e executar um programa simples com classes e objetos.

---

#### **Módulo 2: Elementos Básicos da Linguagem**

- **Conteúdo**:
  - Tipos de dados primitivos e operadores
  - Conversões de tipo
  - Precedência e avaliação de expressões
  - Operadores aritméticos, lógicos e bitwise
- **Exercício**: Implementar cálculos e expressões booleanas.

---

#### **Módulo 3: Declarações e Estruturas de Controle**

- **Conteúdo**:
  - Declarações de classes, métodos e variáveis
  - Sobrecarga de métodos e construtores
  - Arrays e métodos de aridade variável
  - Declarações `if`, `switch`, loops (`for`, `while`, `do-while`)
- **Exemplo**: Implementar um `switch` expression com `yield`.

---

#### **Módulo 4: Programação Orientada a Objetos**

- **Conteúdo**:
  - Herança e polimorfismo
  - Classes abstratas e interfaces
  - Enums, records e sealed classes
  - Sobrescrita e sobrecarga
- **Exercício**: Criar uma hierarquia de classes com herança e interfaces.

---

#### **Módulo 5: Controle de Acesso e Encapsulamento**

- **Conteúdo**:
  - Modificadores de acesso (`public`, `private`, `protected`, `package`)
  - Estrutura de pacotes
  - Imutabilidade
- **Exemplo**: Implementar uma classe imutável.

---

#### **Módulo 6: Tratamento de Exceções**

- **Conteúdo**:
  - Tipos de exceções (verificadas e não verificadas)
  - Blocos `try-catch-finally`
  - `try-with-resources`
  - Lançamento e propagação de exceções
- **Exercício**: Usar `try-with-resources` para gerenciar recursos.

---

#### **Módulo 7: APIs Fundamentais**

- **Conteúdo**:
  - Classes `Object`, `String`, `StringBuilder`
  - Wrapper classes e autoboxing
  - Classes `Math` e `Random`
  - Números grandes (`BigInteger`, `BigDecimal`)
- **Exemplo**: Manipular strings com `StringBuilder`.

---

#### **Módulo 8: Generics e Coleções**

- **Conteúdo**:
  - Tipos genéricos e wildcards
  - Coleções: `ArrayList`, `HashSet`, `LinkedList`, `HashMap`
  - Iteradores e comparadores
- **Exercício**: Implementar uma pilha genérica.

---

#### **Módulo 9: Programação Funcional**

- **Conteúdo**:
  - Interfaces funcionais (`Predicate`, `Consumer`, `Function`, `Supplier`)
  - Expressões lambda e method references
  - Streams: operações intermediárias e terminais
  - Coletores e redução
- **Exemplo**: Processar uma lista com `Streams` e `lambda expressions`.

---

#### **Módulo 10: Data, Hora e Localização**

- **Conteúdo**:
  - API `java.time` (`LocalDate`, `LocalTime`, `ZonedDateTime`)
  - Formatação e análise de datas
  - Internacionalização com `Locale` e `ResourceBundle`
- **Exercício**: Calcular diferenças entre datas usando `Period` e `Duration`.

---

#### **Módulo 11: Sistema de Módulos Java**

- **Conteúdo**:
  - Criação e uso de módulos
  - Diretivas de módulo (`requires`, `exports`)
  - Migração de aplicações para módulos
- **Exemplo**: Criar um aplicativo modular simples.

---

#### **Módulo 12: I/O e NIO.2**

- **Conteúdo**:
  - Leitura e escrita de arquivos com `InputStream`, `OutputStream`
  - Classes `Reader` e `Writer`
  - Uso da API NIO.2 (`Path`, `Files`)
  - Atributos de arquivo e caminhos
- **Exercício**: Ler e escrever arquivos usando `Files.readAllLines()`.

---

#### **Módulo 13: Concorrência**

- **Conteúdo**:
  - Threads e `Runnable`
  - Sincronização e locks
  - `ExecutorService` e `ForkJoinPool`
  - Coleções thread-safe
- **Exemplo**: Implementar um produtor-consumidor com `BlockingQueue`.

---

#### **Módulo 14: JDBC e Anotações**

- **Conteúdo**:
  - Conexão com bancos de dados
  - Execução de consultas e transações
  - Uso de anotações personalizadas e padrão
- **Exercício**: Criar um DAO (Data Access Object) com JDBC.

---

#### **Módulo 15: Segurança em Java**

- **Conteúdo**:
  - Princípios de codificação segura
  - Políticas de segurança e permissões
  - Prevenção de vulnerabilidades comuns
- **Exemplo**: Implementar validação de entrada para evitar SQL injection.

---

#### **Módulo 16: Preparação para o Exame**

- **Conteúdo**:
  - Revisão de tópicos-chave
  - Simulados e questões práticas
  - Estratégias para a prova
- **Recursos**:
  - Appendix E: Mock Exam
  - Appendix F: Respostas comentadas

---

### **Avaliação do Curso**:

- **Questionários** ao final de cada módulo.
- **Projeto Prático**: Desenvolver uma aplicação que utilize os conceitos aprendidos.
- **Simulado Final**: Prova no estilo da certificação.

---

# **Módulo 1: Introdução ao Java e Fundamentos**

## **1.1 Objetivos do Módulo**

- Compreender o ecossistema Java e sua arquitetura
- Dominar a estrutura básica de programas Java
- Entender os conceitos fundamentais de OOP: classes, objetos, instância vs estático
- Implementar herança e agregação na prática
- Preparar o ambiente de desenvolvimento Java

## **1.2 Conteúdo Programático**

### **1.2.1 O Ecossistema Java**

**Conceitos Fundamentais:**

- **Java vs Outras Linguagens**: Linguagem compilada e interpretada
- **JVM (Java Virtual Machine)**: Máquina virtual que executa bytecode
- **JRE (Java Runtime Environment)**: Ambiente de execução
- **JDK (Java Development Kit)**: Kit de desenvolvimento completo

**Arquitetura Java:**

```
Código Fonte (.java) → Compilador → Bytecode (.class) → JVM → Execução
```

### **1.2.2 Estrutura de uma Classe Java**

**Exemplo 1.1: Classe Básica**

```java
// Arquivo: Carro.java
public class Carro {
    // Campos (atributos)
    private String marca;
    private String modelo;
    private int ano;

    // Construtor
    public Carro(String marca, String modelo, int ano) {
        this.marca = marca;
        this.modelo = modelo;
        this.ano = ano;
    }

    // Métodos de instância
    public void exibirInfo() {
        System.out.println("Marca: " + marca);
        System.out.println("Modelo: " + modelo);
        System.out.println("Ano: " + ano);
    }

    // Getters e Setters
    public String getMarca() { return marca; }
    public void setMarca(String marca) { this.marca = marca; }
}
```

### **1.2.3 Objetos e Instâncias**

**Criando e Usando Objetos:**

```java
// Arquivo: Main.java
public class Main {
    public static void main(String[] args) {
        // Criando objetos (instâncias)
        Carro carro1 = new Carro("Toyota", "Corolla", 2023);
        Carro carro2 = new Carro("Honda", "Civic", 2022);

        // Chamando métodos
        carro1.exibirInfo();
        carro2.exibirInfo();
    }
}
```

### **1.2.4 Membros de Instância vs Estáticos**

**Exemplo 1.2: Diferença entre Instância e Estático**

```java
public class Contador {
    // Campo de instância - cada objeto tem sua própria cópia
    private int contadorInstancia;

    // Campo estático - compartilhado por todas as instâncias
    private static int contadorEstatico;

    // Método de instância
    public void incrementarInstancia() {
        contadorInstancia++;
    }

    // Método estático
    public static void incrementarEstatico() {
        contadorEstatico++;
    }

    // Getters
    public int getContadorInstancia() { return contadorInstancia; }
    public static int getContadorEstatico() { return contadorEstatico; }
}

// Uso:
public class TesteContador {
    public static void main(String[] args) {
        Contador c1 = new Contador();
        Contador c2 = new Contador();

        c1.incrementarInstancia(); // Afeta apenas c1
        Contador.incrementarEstatico(); // Afeta todos os objetos

        System.out.println("c1 instância: " + c1.getContadorInstancia()); // 1
        System.out.println("c2 instância: " + c2.getContadorInstancia()); // 0
        System.out.println("Contador estático: " + Contador.getContadorEstatico()); // 1
    }
}
```

### **1.2.5 Herança**

**Exemplo 1.3: Implementando Herança**

```java
// Classe pai (superclasse)
public class Veiculo {
    protected String marca;
    protected String modelo;

    public Veiculo(String marca, String modelo) {
        this.marca = marca;
        this.modelo = modelo;
    }

    public void mover() {
        System.out.println("O veículo está se movendo");
    }
}

// Classe filha (subclasse)
public class Carro extends Veiculo {
    private int numeroPortas;

    public Carro(String marca, String modelo, int numeroPortas) {
        super(marca, modelo); // Chamando construtor da superclasse
        this.numeroPortas = numeroPortas;
    }

    @Override
    public void mover() {
        System.out.println("O carro " + marca + " " + modelo + " está andando na estrada");
    }

    public void abrirPortas() {
        System.out.println("Abrindo " + numeroPortas + " portas");
    }
}
```

### **1.2.6 Agregação**

**Exemplo 1.4: Relação "Tem-um"**

```java
public class Motor {
    private int potencia;
    private String tipoCombustivel;

    public Motor(int potencia, String tipoCombustivel) {
        this.potencia = potencia;
        this.tipoCombustivel = tipoCombustivel;
    }

    public void ligar() {
        System.out.println("Motor ligado - " + potencia + " cavalos");
    }
}

public class CarroComMotor {
    private String modelo;
    private Motor motor; // Agregação - Carro TEM-UM Motor

    public CarroComMotor(String modelo, Motor motor) {
        this.modelo = modelo;
        this.motor = motor;
    }

    public void iniciar() {
        System.out.println("Iniciando carro: " + modelo);
        motor.ligar();
    }
}

// Uso:
public class TesteAgregacao {
    public static void main(String[] args) {
        Motor motorV8 = new Motor(450, "Gasolina");
        CarroComMotor carroEsportivo = new CarroComMotor("Mustang", motorV8);
        carroEsportivo.iniciar();
    }
}
```

## **1.3 Exercícios Práticos**

### **Exercício 1: Sistema Bancário Básico**

```java
public class ContaBancaria {
    private static int totalContas = 0; // Variável estática
    private int numeroConta;
    private String titular;
    private double saldo;

    public ContaBancaria(String titular, double depositoInicial) {
        this.numeroConta = ++totalContas;
        this.titular = titular;
        this.saldo = depositoInicial;
    }

    public void depositar(double valor) {
        saldo += valor;
    }

    public boolean sacar(double valor) {
        if (valor <= saldo) {
            saldo -= valor;
            return true;
        }
        return false;
    }

    public void exibirSaldo() {
        System.out.println("Titular: " + titular);
        System.out.println("Saldo: R$ " + saldo);
    }

    public static int getTotalContas() {
        return totalContas;
    }
}
```

### **Exercício 2: Hierarquia de Funcionários**

```java
public class Funcionario {
    protected String nome;
    protected double salarioBase;

    public Funcionario(String nome, double salarioBase) {
        this.nome = nome;
        this.salarioBase = salarioBase;
    }

    public double calcularSalario() {
        return salarioBase;
    }
}

public class Gerente extends Funcionario {
    private double bonus;

    public Gerente(String nome, double salarioBase, double bonus) {
        super(nome, salarioBase);
        this.bonus = bonus;
    }

    @Override
    public double calcularSalario() {
        return salarioBase + bonus;
    }
}
```

## **1.4 Questionário de Revisão**

**Questão 1:** Qual a diferença entre JVM, JRE e JDK?
- A) JDK inclui JRE que inclui JVM
- B) São a mesma coisa
- C) JVM é para desenvolvimento, JDK para execução

**Questão 2:** O que é um construtor em Java?
- A) Um método especial para inicializar objetos
- B) Um tipo de variável
- C) Uma classe abstrata

**Questão 3:** Qual a saída do código abaixo?

```java
public class Teste {
    static int x = 10;
    int y = 20;
    
    public static void main(String[] args) {
        Teste t1 = new Teste();
        Teste t2 = new Teste();
        t1.x = 100;
        t1.y = 200;
        System.out.println(t2.x + " " + t2.y);
    }
}
```

**Questão 4:** Explique a diferença entre herança e agregação.

## **1.5 Laboratório Prático**

**Projeto: Sistema de Biblioteca Simplificado**

```java
// Implemente as classes:
// 1. Livro (titulo, autor, ISBN)
// 2. Membro (nome, ID, lista de livros emprestados)
// 3. Biblioteca (lista de livros, lista de membros, métodos para empréstimo e devolução)

// Use herança para diferentes tipos de membros (Estudante, Professor)
// Use agregação entre Biblioteca, Livro e Membro
```

## **1.6 Material de Apoio**

**Links Úteis:**
- [Documentação Oficial Java SE 17](https://docs.oracle.com/en/java/javase/17/)
- [JDK Download](https://www.oracle.com/java/technologies/javase-downloads.html)
- [Eclipse IDE](https://www.eclipse.org/downloads/)

**Ferramentas Recomendadas:**
- IDE: Eclipse ou IntelliJ IDEA
- JDK 17 ou superior
- Git para controle de versão

## **1.7 Próximos Passos**

No próximo módulo, abordaremos:
- Tipos de dados primitivos e operadores
- Controle de fluxo (if, switch, loops)
- Arrays e manipulação de dados

---

Perfeito! Vamos para o **Módulo 2: Elementos Básicos da Linguagem Java**.

---

# **Módulo 2: Elementos Básicos da Linguagem Java**

## **2.1 Objetivos do Módulo**

- Dominar os tipos de dados primitivos do Java
- Compreender operadores e suas precedências
- Aprender conversões de tipos (casting)
- Trabalhar com operadores aritméticos, lógicos e bitwise
- Entender a avaliação de expressões

## **2.2 Conteúdo Programático**

### **2.2.1 Tipos de Dados Primitivos**

**Tabela 2.1: Tipos Primitivos do Java**

```java
public class TiposPrimitivos {
    public static void main(String[] args) {
        // Tipos inteiros
        byte byteVar = 127; // 8-bit (-128 a 127)
        short shortVar = 32767; // 16-bit (-32,768 a 32,767)
        int intVar = 2147483647; // 32-bit (-2^31 a 2^31-1)
        long longVar = 9223372036854775807L; // 64-bit (sufixo L)

        // Tipos de ponto flutuante
        float floatVar = 3.14f; // 32-bit (sufixo f)
        double doubleVar = 3.141592653589793; // 64-bit

        // Outros tipos
        char charVar = 'A'; // 16-bit Unicode
        boolean boolVar = true; // true ou false

        System.out.println("byte: " + byteVar);
        System.out.println("char: " + charVar + " (Unicode: " + (int)charVar + ")");
    }
}
```

### **2.2.2 Literais em Java**

**Exemplo 2.2: Diferentes Formas de Literais**

```java
public class Literais {
    public static void main(String[] args) {
        // Literais inteiros
        int decimal = 100;
        int octal = 0144; // Prefixo 0 (8*8 + 4*8 + 4 = 100)
        int hexadecimal = 0x64; // Prefixo 0x (6*16 + 4 = 100)
        int binario = 0b1100100; // Prefixo 0b

        // Literais de ponto flutuante
        double double1 = 123.45;
        double double2 = 1.2345e2; // Notação científica (1.2345 × 10²)
        double double3 = 123.45d; // Sufixo d (opcional)

        // Literais de caracteres
        char char1 = 'A';
        char char2 = '\u0041'; // Unicode para 'A'
        char char3 = 65; // Código ASCII

        // Sequências de escape
        System.out.println("Nova linha:\nTexto após nova linha");
        System.out.println("Tab:\tTexto após tab");
        System.out.println("Aspas: \"Texto entre aspas\"");
        System.out.println("Barra invertida: \\");
        System.out.println("Binário 1100100 = " + binario);
        System.out.println("Unicode \\u0041 = " + char2);
    }
}
```

### **2.2.3 Operadores Aritméticos**

**Exemplo 2.3: Operações Aritméticas**

```java
public class OperadoresAritmeticos {
    public static void main(String[] args) {
        int a = 10, b = 3;

        // Operações básicas
        System.out.println("a + b = " + (a + b)); // 13
        System.out.println("a - b = " + (a - b)); // 7
        System.out.println("a * b = " + (a * b)); // 30
        System.out.println("a / b = " + (a / b)); // 3 (divisão inteira)
        System.out.println("a % b = " + (a % b)); // 1 (resto da divisão)

        // Divisão com ponto flutuante
        System.out.println("a / b (float) = " + ((float)a / b)); // 3.333...

        // Incremento e decremento
        int x = 5;
        System.out.println("x++ = " + x++); // 5 (pós-incremento)
        System.out.println("x = " + x); // 6
        System.out.println("++x = " + ++x); // 7 (pré-incremento)

        // Operadores compostos
        int y = 10;
        y += 5; // Equivalente a y = y + 5
        System.out.println("y += 5 → " + y); // 15
    }
}
```

### **2.2.4 Conversões de Tipo (Casting)**

**Exemplo 2.4: Conversões Implícitas e Explícitas**

```java
public class Conversoes {
    public static void main(String[] args) {
        // Conversão implícita (widening)
        int intVal = 100;
        long longVal = intVal; // Conversão automática
        double doubleVal = intVal; // Conversão automática

        System.out.println("int para long: " + longVal);
        System.out.println("int para double: " + doubleVal);

        // Conversão explícita (narrowing) - requer cast
        double d = 99.99;
        int i = (int) d; // Cast explícito (trunca a parte decimal)
        byte b = (byte) 200; // Overflow (200 > 127)

        System.out.println("double 99.99 para int: " + i); // 99
        System.out.println("200 para byte: " + b); // -56 (overflow)

        // Promoção numérica em expressões
        byte byte1 = 10;
        byte byte2 = 20;
        // byte result = byte1 + byte2; // ERRO! Resultado é int
        int result = byte1 + byte2; // Correto
        byte resultCast = (byte)(byte1 + byte2); // Com cast

        System.out.println("byte + byte = int: " + result);
    }
}
```

### **2.2.5 Precedência de Operadores**

**Tabela 2.2: Precedência de Operadores**

```java
public class Precedencia {
    public static void main(String[] args) {
        int a = 10, b = 5, c = 2;

        // Diferentes precedências
        int resultado1 = a + b * c; // 10 + (5 * 2) = 20
        int resultado2 = (a + b) * c; // (10 + 5) * 2 = 30
        int resultado3 = a + b / c; // 10 + (5 / 2) = 12
        int resultado4 = a * b / c; // (10 * 5) / 2 = 25

        System.out.println("a + b * c = " + resultado1);
        System.out.println("(a + b) * c = " + resultado2);
        System.out.println("a + b / c = " + resultado3);
        System.out.println("a * b / c = " + resultado4);

        // Precedência com operadores lógicos
        boolean x = true, y = false, z = true;
        boolean logico1 = x || y && z; // true || (false && true) = true
        boolean logico2 = (x || y) && z; // (true || false) && true = true

        System.out.println("x || y && z = " + logico1);
        System.out.println("(x || y) && z = " + logico2);
    }
}
```

### **2.2.6 Operadores Relacionais e Lógicos**

**Exemplo 2.5: Operadores de Comparação**

```java
public class OperadoresRelacionais {
    public static void main(String[] args) {
        int a = 10, b = 5, c = 10;

        // Operadores relacionais
        System.out.println(a + " == " + c + " : " + (a == c)); // true
        System.out.println(a + " != " + b + " : " + (a != b)); // true
        System.out.println(a + " > " + b + " : " + (a > b)); // true
        System.out.println(a + " < " + b + " : " + (a < b)); // false
        System.out.println(a + " >= " + c + " : " + (a >= c)); // true

        // Operadores lógicos
        boolean x = true, y = false;
        System.out.println("x && y : " + (x && y)); // AND - false
        System.out.println("x || y : " + (x || y)); // OR - true
        System.out.println("!x : " + (!x)); // NOT - false

        // Curto-circuito (short-circuit)
        int count = 0;
        boolean result = (count != 0) && (100 / count > 0); // Evita divisão por zero
        System.out.println("Resultado com short-circuit: " + result);
    }
}
```

### **2.2.7 Operadores Bitwise**

**Exemplo 2.6: Operações Bit a Bit**

```java
public class OperadoresBitwise {
    public static void main(String[] args) {
        int a = 5; // 0101 em binário
        int b = 3; // 0011 em binário

        System.out.println("a = " + a + " (binário: " + Integer.toBinaryString(a) + ")");
        System.out.println("b = " + b + " (binário: " + Integer.toBinaryString(b) + ")");

        // Operadores bitwise
        System.out.println("a & b : " + (a & b) + " (AND - 0001)"); // 1
        System.out.println("a | b : " + (a | b) + " (OR - 0111)"); // 7
        System.out.println("a ^ b : " + (a ^ b) + " (XOR - 0110)"); // 6
        System.out.println("~a : " + (~a) + " (NOT)"); // -6
        System.out.println("a << 1 : " + (a << 1) + " (shift left - 1010)"); // 10
        System.out.println("a >> 1 : " + (a >> 1) + " (shift right - 0010)"); // 2

        // Aplicação prática: verificar se um número é par
        int numero = 8;
        boolean isPar = (numero & 1) == 0; // Último bit 0 = par
        System.out.println(numero + " é par? " + isPar);
    }
}
```

### **2.2.8 Operador Ternário**

**Exemplo 2.7: Operador Condicional Ternário**

```java
public class OperadorTernario {
    public static void main(String[] args) {
        int nota = 75;

        // Sintaxe: condição ? valor_se_verdadeiro : valor_se_falso
        String resultado = nota >= 70 ? "Aprovado" : "Reprovado";
        System.out.println("Nota " + nota + ": " + resultado);

        // Ternário aninhado
        int score = 85;
        String conceito = score >= 90 ? "A" :
                         score >= 80 ? "B" :
                         score >= 70 ? "C" : "D";

        System.out.println("Score " + score + ": Conceito " + conceito);

        // Uso em atribuição
        int max = (a > b) ? a : b;
        System.out.println("Máximo entre " + a + " e " + b + ": " + max);
    }
}
```

## **2.3 Exercícios Práticos**

### **Exercício 2.1: Calculadora de IMC**

```java
public class CalculadoraIMC {
    public static void main(String[] args) {
        double peso = 70.5; // kg
        double altura = 1.75; // metros

        // Calcular IMC: peso / (altura * altura)
        double imc = peso / (altura * altura);

        System.out.printf("Peso: %.1f kg\n", peso);
        System.out.printf("Altura: %.2f m\n", altura);
        System.out.printf("IMC: %.2f\n", imc);

        // Classificação usando operadores lógicos
        if (imc < 18.5) {
            System.out.println("Classificação: Abaixo do peso");
        } else if (imc < 25) {
            System.out.println("Classificação: Peso normal");
        } else if (imc < 30) {
            System.out.println("Classificação: Sobrepeso");
        } else {
            System.out.println("Classificação: Obesidade");
        }
    }
}
```

### **Exercício 2.2: Conversor de Temperatura**

```java
public class ConversorTemperatura {
    public static void main(String[] args) {
        double celsius = 25.0;

        // Converter para Fahrenheit: (C × 9/5) + 32
        double fahrenheit = (celsius * 9 / 5) + 32;

        // Converter para Kelvin: C + 273.15
        double kelvin = celsius + 273.15;

        System.out.printf("%.1f°C = %.1f°F\n", celsius, fahrenheit);
        System.out.printf("%.1f°C = %.1fK\n", celsius, kelvin);

        // Usando operadores bitwise para demonstração
        int tempInt = (int) celsius;
        System.out.println("Temperatura em binário: " + Integer.toBinaryString(tempInt));
    }
}
```

### **Exercício 2.3: Manipulação de Bits**

```java
public class ManipulacaoBits {
    public static void main(String[] args) {
        int flags = 0b1010; // 10 em decimal

        // Verificar bits específicos
        boolean bit3 = (flags & 0b1000) != 0; // Terceiro bit
        boolean bit1 = (flags & 0b0010) != 0; // Primeiro bit

        System.out.println("Flags: " + Integer.toBinaryString(flags));
        System.out.println("Bit 3 está setado? " + bit3);
        System.out.println("Bit 1 está setado? " + bit1);

        // Setar um bit
        int newFlags = flags | 0b0001; // Setar bit 0
        System.out.println("Novas flags: " + Integer.toBinaryString(newFlags));

        // Limpar um bit
        newFlags = newFlags & ~0b1000; // Limpar bit 3
        System.out.println("Flags após limpar bit 3: " + Integer.toBinaryString(newFlags));
    }
}
```

## **2.4 Caso Prático: Sistema de Verificação de Elegibilidade**

```java
public class VerificadorElegibilidade {
    public static void main(String[] args) {
        int idade = 25;
        double renda = 45000.0;
        boolean temEmprego = true;
        int scoreCredito = 750;

        // Regras de elegibilidade usando operadores lógicos
        boolean elegivelIdade = idade >= 18 && idade <= 65;
        boolean elegivelRenda = renda >= 30000.0;
        boolean elegivelScore = scoreCredito >= 700;

        // Elegibilidade geral
        boolean elegivel = elegivelIdade && elegivelRenda && temEmprego && elegivelScore;

        System.out.println("Idade: " + idade + " - Elegível: " + elegivelIdade);
        System.out.println("Renda: $" + renda + " - Elegível: " + elegivelRenda);
        System.out.println("Score: " + scoreCredito + " - Elegível: " + elegivelScore);
        System.out.println("Tem emprego: " + temEmprego);
        System.out.println("Elegível geral: " + elegivel);

        // Mensagem detalhada usando operador ternário
        String mensagem = elegivel ?
            "Parabéns! Você está elegível para o empréstimo." :
            "Infelizmente você não atende aos critérios de elegibilidade.";

        System.out.println(mensagem);
    }
}
```

## **2.5 Questionário de Revisão**

**Questão 1:** Qual o resultado de `10 / 3` em Java?
- A) 3.333...
- B) 3
- C) 3.0
- D) Erro de compilação

**Questão 2:** O que acontece ao converter `double d = 100.99; int i = (int) d;`?
- A) i = 100
- B) i = 101
- C) i = 100.99
- D) Erro de compilação

**Questão 3:** Qual a precedência correta?
- A) `* / %` > `+ -` > `&&` > `||`
- B) `&&` > `||` > `* / %` > `+ -`
- C) `+ -` > `* / %` > `&&` > `||`

**Questão 4:** Qual o resultado de `5 & 3`?
- A) 7
- B) 1
- C) 6
- D) 0

**Questão 5:** O que é short-circuit evaluation?

## **2.6 Laboratório Prático**

**Projeto: Calculadora Científica Básica**

```java
// Implemente uma calculadora que inclua:
// 1. Operações básicas (+, -, *, /, %)
// 2. Conversão entre decimal, binário, hexadecimal
// 3. Operações bitwise (&, |, ^, ~, <<, >>)
// 4. Cálculo de potência e raiz quadrada
// 5. Verificação de números primos

// Dica: Use Math.pow(), Math.sqrt(), Integer.toBinaryString()
```

## **2.7 Desafios Avançados**

**Desafio 1: Criptografia Simples**

```java
public class CriptografiaSimples {
    public static void main(String[] args) {
        String mensagem = "HELLO";
        int chave = 5;

        // Cifra de César usando operações com chars
        StringBuilder cifrado = new StringBuilder();
        for (char c : mensagem.toCharArray()) {
            if (Character.isLetter(c)) {
                char base = Character.isUpperCase(c) ? 'A' : 'a';
                char cifradoChar = (char)(((c - base + chave) % 26) + base);
                cifrado.append(cifradoChar);
            } else {
                cifrado.append(c);
            }
        }

        System.out.println("Original: " + mensagem);
        System.out.println("Cifrado: " + cifrado);
    }
}
```

**Desafio 2: Verificador de Palíndromo Numérico**

```java
public class PalindromoNumerico {
    public static void main(String[] args) {
        int numero = 12321;
        int original = numero;
        int reverso = 0;

        // Inverter o número usando operações matemáticas
        while (numero != 0) {
            int digito = numero % 10;
            reverso = reverso * 10 + digito;
            numero /= 10;
        }

        boolean ehPalindromo = (original == reverso);
        System.out.println(original + " é palíndromo? " + ehPalindromo);
    }
}
```

## **2.8 Material de Apoio**

**Resumo dos Operadores:**
- **Aritméticos**: `+ - * / % ++ --`
- **Relacionais**: `== != > < >= <=`
- **Lógicos**: `&& || ! ^`
- **Bitwise**: `& | ^ ~ << >> >>>`
- **Atribuição**: `= += -= *= /= %= &= |= ^= <<= >>=`
- **Ternário**: `? :`

**Dicas Importantes:**
- Divisão inteira trunca a parte decimal
- Overflow ocorre silenciosamente em Java
- Use parênteses para clarificar precedência
- `&&` e `||` têm short-circuit evaluation

---

**Próximo Módulo: Declarações e Estruturas de Controle**

Excelente! Vamos para o **Módulo 3: Declarações e Estruturas de Controle**. Este é um módulo crucial onde aplicaremos todos os operadores aprendidos anteriormente em estruturas de controle reais.

---

# **Módulo 3: Declarações e Estruturas de Controle**

## **3.1 Objetivos do Módulo**

- Dominar estruturas de decisão: `if-else`, `switch`
- Compreender loops: `for`, `while`, `do-while`
- Aprender a usar `break`, `continue` e labels
- Trabalhar com arrays e enhanced for loop
- Entender declarações de variáveis e escopo

## **3.2 Conteúdo Programático**

### **3.2.1 Declarações de Variáveis e Escopo**

**Exemplo 3.1: Escopo de Variáveis**

```java
public class EscopoVariaveis {
    // Variável de instância - escopo de objeto
    private int variavelInstancia = 10;

    public void metodoExemplo(int parametro) { // parâmetro - escopo do método
        // Variável local - escopo do método
        int variavelLocalMetodo = 20;

        if (parametro > 0) {
            // Variável de bloco - escopo do bloco if
            int variavelBloco = 30;
            System.out.println("Variável de bloco: " + variavelBloco);
            System.out.println("Variável local do método: " + variavelLocalMetodo);
            System.out.println("Variável de instância: " + variavelInstancia);
        }
        // System.out.println(variavelBloco); // ERRO! Fora do escopo
    }

    public static void main(String[] args) {
        EscopoVariaveis obj = new EscopoVariaveis();
        obj.metodoExemplo(5);

        // Inferência de tipo com var (Java 10+)
        var nome = "João Silva";
        var idade = 25;
        var salario = 2500.50;

        System.out.println("Nome: " + nome + ", Tipo: " + nome.getClass().getSimpleName());
        System.out.println("Idade: " + idade + ", Tipo: int");
        System.out.println("Salário: " + salario + ", Tipo: double");
    }
}
```

### **3.2.2 Estruturas de Decisão: if-else**

**Exemplo 3.2: Declarações if-else**

```java
public class ControleIfElse {
    public static void main(String[] args) {
        int nota = 85;

        // if simples
        if (nota >= 70) {
            System.out.println("Aprovado");
        }

        // if-else
        if (nota >= 70) {
            System.out.println("Aprovado");
        } else {
            System.out.println("Reprovado");
        }

        // else-if
        if (nota >= 90) {
            System.out.println("Conceito A");
        } else if (nota >= 80) {
            System.out.println("Conceito B");
        } else if (nota >= 70) {
            System.out.println("Conceito C");
        } else {
            System.out.println("Conceito F");
        }

        // if aninhado
        int idade = 20;
        boolean temCarteira = true;

        if (idade >= 18) {
            if (temCarteira) {
                System.out.println("Pode dirigir");
            } else {
                System.out.println("Precisa de carteira");
            }
        } else {
            System.out.println("Menor de idade");
        }

        // Operador ternário em ação
        String status = (nota >= 70) ? "Aprovado" : "Reprovado";
        System.out.println("Status: " + status);
    }
}
```

### **3.2.3 Declaração switch tradicional**

**Exemplo 3.3: Switch com Colons**

```java
public class SwitchTraditional {
    public static void main(String[] args) {
        int diaSemana = 3;
        String nomeDia;

        switch (diaSemana) {
            case 1:
                nomeDia = "Domingo";
                break;
            case 2:
                nomeDia = "Segunda";
                break;
            case 3:
                nomeDia = "Terça";
                break;
            case 4:
                nomeDia = "Quarta";
                break;
            case 5:
                nomeDia = "Quinta";
                break;
            case 6:
                nomeDia = "Sexta";
                break;
            case 7:
                nomeDia = "Sábado";
                break;
            default:
                nomeDia = "Dia inválido";
        }

        System.out.println("Dia " + diaSemana + ": " + nomeDia);

        // Fall-through intencional
        int mes = 2;
        int ano = 2020;
        int numDias = 0;

        switch (mes) {
            case 1: case 3: case 5: case 7: case 8: case 10: case 12:
                numDias = 31;
                break;
            case 4: case 6: case 9: case 11:
                numDias = 30;
                break;
            case 2:
                if (((ano % 4 == 0) && !(ano % 100 == 0)) || (ano % 400 == 0)) {
                    numDias = 29;
                } else {
                    numDias = 28;
                }
                break;
            default:
                System.out.println("Mês inválido");
        }

        System.out.println("Mês " + mes + " tem " + numDias + " dias");
    }
}
```

### **3.2.4 Expressão switch (Java 14+)**

**Exemplo 3.4: Switch Expressions**

```java
public class SwitchExpression {
    public static void main(String[] args) {
        int diaSemana = 3;

        // Switch expression com arrow ->
        String nomeDia = switch (diaSemana) {
            case 1 -> "Domingo";
            case 2 -> "Segunda";
            case 3 -> "Terça";
            case 4 -> "Quarta";
            case 5 -> "Quinta";
            case 6 -> "Sexta";
            case 7 -> "Sábado";
            default -> "Dia inválido";
        };

        System.out.println("Dia " + diaSemana + ": " + nomeDia);

        // Switch expression com yield (para múltiplas linhas)
        String tipoDia = switch (diaSemana) {
            case 1, 7 -> {
                yield "Fim de semana";
            }
            case 2, 3, 4, 5, 6 -> {
                yield "Dia útil";
            }
            default -> throw new IllegalArgumentException("Dia inválido: " + diaSemana);
        };

        System.out.println("Dia " + diaSemana + " é: " + tipoDia);

        // Usando switch expression para retornar valores
        int numero = 5;
        String parOuImpar = switch (numero % 2) {
            case 0 -> "Par";
            case 1 -> "Ímpar";
            default -> "Inválido";
        };

        System.out.println(numero + " é " + parOuImpar);
    }
}
```

### **3.2.5 Switch com Strings e Enums**

**Exemplo 3.5: Switch Avançado**

```java
// Enum para exemplo
enum NivelPrioridade {
    BAIXA, MEDIA, ALTA, URGENTE
}

public class SwitchAvancado {
    public static void main(String[] args) {
        // Switch com Strings (Java 7+)
        String linguagem = "Java";
        switch (linguagem.toLowerCase()) {
            case "java":
                System.out.println("Linguagem orientada a objetos");
                break;
            case "python":
                System.out.println("Linguagem de script");
                break;
            case "c++":
                System.out.println("Linguagem de sistemas");
                break;
            default:
                System.out.println("Linguagem desconhecida");
        }

        // Switch com Enums
        NivelPrioridade prioridade = NivelPrioridade.ALTA;
        String acao = switch (prioridade) {
            case BAIXA -> "Processar quando possível";
            case MEDIA -> "Processar esta semana";
            case ALTA -> "Processar hoje";
            case URGENTE -> "Processar imediatamente";
        };

        System.out.println("Prioridade " + prioridade + ": " + acao);
    }
}
```

### **3.2.6 Loops: for, while, do-while**

**Exemplo 3.6: Estruturas de Repetição**

```java
public class EstruturasRepeticao {
    public static void main(String[] args) {
        // for loop tradicional
        System.out.println("For loop:");
        for (int i = 1; i <= 5; i++) {
            System.out.println("Contador: " + i);
        }

        // while loop
        System.out.println("\nWhile loop:");
        int j = 1;
        while (j <= 5) {
            System.out.println("Contador: " + j);
            j++;
        }

        // do-while loop (executa pelo menos uma vez)
        System.out.println("\nDo-while loop:");
        int k = 1;
        do {
            System.out.println("Contador: " + k);
            k++;
        } while (k <= 5);

        // Loop infinito com break
        System.out.println("\nLoop com break:");
        int contador = 1;
        while (true) {
            System.out.println("Contador: " + contador);
            if (contador >= 3) {
                break;
            }
            contador++;
        }

        // Loop com continue
        System.out.println("\nLoop com continue (números ímpares):");
        for (int i = 1; i <= 10; i++) {
            if (i % 2 == 0) {
                continue; // Pula números pares
            }
            System.out.println("Número ímpar: " + i);
        }
    }
}
```

### **3.2.7 Enhanced for loop (for-each)**

**Exemplo 3.7: For-Each Loop**

```java
import java.util.Arrays;
import java.util.List;

public class ForEachLoop {
    public static void main(String[] args) {
        // Array tradicional
        int[] numeros = {1, 2, 3, 4, 5};

        // For-each com array
        System.out.println("Array com for-each:");
        for (int numero : numeros) {
            System.out.println("Número: " + numero);
        }

        // Lista com for-each
        List<String> frutas = Arrays.asList("Maçã", "Banana", "Laranja");
        System.out.println("\nLista com for-each:");
        for (String fruta : frutas) {
            System.out.println("Fruta: " + fruta);
        }

        // For-each com matriz
        int[][] matriz = {{1, 2, 3}, {4, 5, 6}, {7, 8, 9}};
        System.out.println("\nMatriz com for-each:");
        for (int[] linha : matriz) {
            for (int elemento : linha) {
                System.out.print(elemento + " ");
            }
            System.out.println();
        }
    }
}
```

### **3.2.8 Break e Continue com Labels**

**Exemplo 3.8: Labels em Loops**

```java
public class LabelsLoops {
    public static void main(String[] args) {
        // Break com label
        System.out.println("Break com label:");
        externo: for (int i = 1; i <= 3; i++) {
            for (int j = 1; j <= 3; j++) {
                if (i == 2 && j == 2) {
                    break externo; // Sai do loop externo
                }
                System.out.println("i=" + i + ", j=" + j);
            }
        }

        // Continue com label
        System.out.println("\nContinue com label:");
        externo: for (int i = 1; i <= 3; i++) {
            for (int j = 1; j <= 3; j++) {
                if (i == 2 && j == 2) {
                    continue externo; // Continua com próxima iteração do loop externo
                }
                System.out.println("i=" + i + ", j=" + j);
            }
        }

        // Exemplo prático: busca em matriz
        int[][] matriz = {{1, 2, 3}, {4, 5, 6}, {7, 8, 9}};
        int alvo = 5;
        boolean encontrado = false;

        busca: for (int i = 0; i < matriz.length; i++) {
            for (int j = 0; j < matriz[i].length; j++) {
                if (matriz[i][j] == alvo) {
                    encontrado = true;
                    System.out.println("Encontrado " + alvo + " em [" + i + "][" + j + "]");
                    break busca;
                }
            }
        }

        if (!encontrado) {
            System.out.println(alvo + " não encontrado na matriz");
        }
    }
}
```

### **3.2.9 Trabalhando com Arrays**

**Exemplo 3.9: Manipulação de Arrays**

```java
import java.util.Arrays;

public class ManipulacaoArrays {
    public static void main(String[] args) {
        // Declaração e inicialização de arrays
        int[] numeros1 = new int[5]; // Array de 5 elementos (todos 0)
        int[] numeros2 = {1, 2, 3, 4, 5}; // Array inicializado
        int[] numeros3 = new int[]{6, 7, 8, 9, 10}; // Outra forma

        // Acessando e modificando elementos
        numeros1[0] = 10;
        numeros1[1] = 20;

        System.out.println("Array numeros1: " + Arrays.toString(numeros1));
        System.out.println("Array numeros2: " + Arrays.toString(numeros2));
        System.out.println("Tamanho do array: " + numeros2.length);

        // Percorrendo array com for tradicional
        System.out.println("\nPercorrendo com for:");
        for (int i = 0; i < numeros2.length; i++) {
            System.out.println("Elemento " + i + ": " + numeros2[i]);
        }

        // Array multidimensional
        int[][] matriz = {
            {1, 2, 3},
            {4, 5, 6},
            {7, 8, 9}
        };

        System.out.println("\nMatriz:");
        for (int i = 0; i < matriz.length; i++) {
            for (int j = 0; j < matriz[i].length; j++) {
                System.out.print(matriz[i][j] + " ");
            }
            System.out.println();
        }

        // Operações com arrays
        int[] copia = Arrays.copyOf(numeros2, 3);
        System.out.println("\nCópia parcial: " + Arrays.toString(copia));

        Arrays.sort(copia);
        System.out.println("Cópia ordenada: " + Arrays.toString(copia));

        int indice = Arrays.binarySearch(copia, 3);
        System.out.println("Índice do elemento 3: " + indice);
    }
}
```

## **3.3 Exercícios Práticos**

### **Exercício 3.1: Calculadora de Fatorial**

```java
public class Fatorial {
    public static void main(String[] args) {
        int numero = 5;
        long fatorial = 1;

        // Calculando fatorial com for
        for (int i = 1; i <= numero; i++) {
            fatorial *= i;
        }

        System.out.println("Fatorial de " + numero + " é: " + fatorial);

        // Versão com while
        fatorial = 1;
        int i = 1;
        while (i <= numero) {
            fatorial *= i;
            i++;
        }

        System.out.println("Fatorial (while) de " + numero + " é: " + fatorial);

        // Versão recursiva (para demonstrar diferentes abordagens)
        System.out.println("Fatorial (recursivo) de " + numero + " é: " + fatorialRecursivo(numero));
    }

    public static long fatorialRecursivo(int n) {
        if (n <= 1) return 1;
        return n * fatorialRecursivo(n - 1);
    }
}
```

### **Exercício 3.2: Verificador de Números Primos**

```java
public class VerificadorPrimo {
    public static void main(String[] args) {
        int numero = 17;
        boolean ehPrimo = true;

        if (numero <= 1) {
            ehPrimo = false;
        } else {
            // Verifica divisores até a raiz quadrada do número
            for (int i = 2; i <= Math.sqrt(numero); i++) {
                if (numero % i == 0) {
                    ehPrimo = false;
                    break;
                }
            }
        }

        System.out.println(numero + (ehPrimo ? " é primo" : " não é primo"));

        // Encontrar todos os primos até 50
        System.out.println("\nNúmeros primos até 50:");
        for (int i = 2; i <= 50; i++) {
            boolean primo = true;
            for (int j = 2; j <= Math.sqrt(i); j++) {
                if (i % j == 0) {
                    primo = false;
                    break;
                }
            }
            if (primo) {
                System.out.print(i + " ");
            }
        }
    }
}
```

### **Exercício 3.3: Sistema de Menu Interativo**

```java
import java.util.Scanner;

public class MenuInterativo {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        int opcao;

        do {
            System.out.println("\n=== MENU PRINCIPAL ===");
            System.out.println("1. Calcular IMC");
            System.out.println("2. Verificar número primo");
            System.out.println("3. Calcular fatorial");
            System.out.println("4. Tabuada");
            System.out.println("0. Sair");
            System.out.print("Escolha uma opção: ");

            opcao = scanner.nextInt();

            switch (opcao) {
                case 1:
                    System.out.print("Digite o peso (kg): ");
                    double peso = scanner.nextDouble();
                    System.out.print("Digite a altura (m): ");
                    double altura = scanner.nextDouble();
                    double imc = peso / (altura * altura);
                    System.out.printf("Seu IMC: %.2f\n", imc);
                    break;

                case 2:
                    System.out.print("Digite um número: ");
                    int num = scanner.nextInt();
                    boolean primo = true;
                    for (int i = 2; i <= Math.sqrt(num); i++) {
                        if (num % i == 0) {
                            primo = false;
                            break;
                        }
                    }
                    System.out.println(num + (primo ? " é primo" : " não é primo"));
                    break;

                case 3:
                    System.out.print("Digite um número: ");
                    int n = scanner.nextInt();
                    long fat = 1;
                    for (int i = 1; i <= n; i++) {
                        fat *= i;
                    }
                    System.out.println(n + "! = " + fat);
                    break;

                case 4:
                    System.out.print("Digite um número para tabuada: ");
                    int base = scanner.nextInt();
                    for (int i = 1; i <= 10; i++) {
                        System.out.println(base + " x " + i + " = " + (base * i));
                    }
                    break;

                case 0:
                    System.out.println("Saindo...");
                    break;

                default:
                    System.out.println("Opção inválida!");
            }
        } while (opcao != 0);

        scanner.close();
    }
}
```

## **3.4 Caso Prático: Jogo de Adivinhação**

```java
import java.util.Random;
import java.util.Scanner;

public class JogoAdivinhacao {
    public static void main(String[] args) {
        Random random = new Random();
        Scanner scanner = new Scanner(System.in);

        int numeroSecreto = random.nextInt(100) + 1; // 1-100
        int tentativas = 0;
        int maxTentativas = 7;
        boolean acertou = false;

        System.out.println("=== JOGO DE ADIVINHAÇÃO ===");
        System.out.println("Tente adivinhar o número entre 1 e 100");
        System.out.println("Você tem " + maxTentativas + " tentativas!");

        while (tentativas < maxTentativas && !acertou) {
            System.out.print("\nTentativa " + (tentativas + 1) + ": ");
            int palpite = scanner.nextInt();
            tentativas++;

            if (palpite == numeroSecreto) {
                acertou = true;
                System.out.println("PARABÉNS! Você acertou em " + tentativas + " tentativas!");
            } else if (palpite < numeroSecreto) {
                System.out.println("O número secreto é MAIOR que " + palpite);
            } else {
                System.out.println("O número secreto é MENOR que " + palpite);
            }

            // Dica após algumas tentativas
            if (tentativas == 3 && !acertou) {
                String dica = (numeroSecreto % 2 == 0) ? "par" : "ímpar";
                System.out.println("DICA: O número é " + dica + "!");
            }
        }

        if (!acertou) {
            System.out.println("\nGame Over! O número era: " + numeroSecreto);
        }

        scanner.close();
    }
}
```

## **3.5 Questionário de Revisão**

**Questão 1:** Qual a diferença entre `break` e `continue`?
- A) `break` sai do loop, `continue` pula para próxima iteração
- B) Ambos fazem a mesma coisa
- C) `break` funciona apenas em switch

**Questão 2:** O que é fall-through em switch?
- A) Quando não se usa `break` e execução continua no próximo case
- B) Erro de compilação
- C) Quando o switch não tem default

**Questão 3:** Qual loop executa pelo menos uma vez?
- A) for
- B) while
- C) do-while

**Questão 4:** O que este código imprime?

```java
for (int i = 0; i < 3; i++) {
    if (i == 1) continue;
    System.out.print(i + " ");
}
```

**Questão 5:** Qual a vantagem do switch expression sobre switch statement?

## **3.6 Laboratório Prático**

**Projeto: Sistema de Análise de Notas**

```java
import java.util.Arrays;

public class AnaliseNotas {
    public static void main(String[] args) {
        double[] notas = {7.5, 8.0, 6.5, 9.0, 5.5, 7.0, 8.5, 4.0, 6.0, 9.5};

        // 1. Calcular média
        double soma = 0;
        for (double nota : notas) {
            soma += nota;
        }
        double media = soma / notas.length;

        // 2. Encontrar maior e menor nota
        double maior = notas[0];
        double menor = notas[0];
        for (int i = 1; i < notas.length; i++) {
            if (notas[i] > maior) maior = notas[i];
            if (notas[i] < menor) menor = notas[i];
        }

        // 3. Contar aprovados (nota >= 7.0)
        int aprovados = 0;
        for (double nota : notas) {
            if (nota >= 7.0) aprovados++;
        }

        // 4. Classificar conceitos
        String[] conceitos = new String[notas.length];
        for (int i = 0; i < notas.length; i++) {
            conceitos[i] = switch ((int) notas[i]) {
                case 10, 9 -> "A";
                case 8 -> "B";
                case 7 -> "C";
                case 6 -> "D";
                default -> "F";
            };
        }

        // 5. Exibir resultados
        System.out.println("=== ANÁLISE DE NOTAS ===");
        System.out.println("Notas: " + Arrays.toString(notas));
        System.out.println("Média da turma: " + media);
        System.out.println("Maior nota: " + maior);
        System.out.println("Menor nota: " + menor);
        System.out.println("Aprovados: " + aprovados + "/" + notas.length);
        System.out.println("Conceitos: " + Arrays.toString(conceitos));

        // 6. Histograma
        System.out.println("\nHISTOGRAMA:");
        for (int i = 0; i <= 10; i++) {
            int count = 0;
            for (double nota : notas) {
                if ((int) nota == i) count++;
            }
            System.out.println(i + ": " + "*".repeat(count));
        }
    }
}
```

## **3.7 Desafios Avançados**

**Desafio 1: Torre de Hanoi**

```java
public class TorreHanoi {
    public static void resolver(int discos, char origem, char destino, char auxiliar) {
        if (discos == 1) {
            System.out.println("Mover disco 1 de " + origem + " para " + destino);
            return;
        }

        resolver(discos - 1, origem, auxiliar, destino);
        System.out.println("Mover disco " + discos + " de " + origem + " para " + destino);
        resolver(discos - 1, auxiliar, destino, origem);
    }

    public static void main(String[] args) {
        int discos = 3;
        System.out.println("Solução da Torre de Hanoi com " + discos + " discos:");
        resolver(discos, 'A', 'C', 'B');
    }
}
```

**Desafio 2: Gerador de Sequência de Fibonacci**

```java
public class Fibonacci {
    public static void main(String[] args) {
        int n = 10;

        System.out.println("Sequência de Fibonacci até " + n + " termos:");

        // Usando array
        int[] fib = new int[n];
        fib[0] = 0;
        fib[1] = 1;

        for (int i = 2; i < n; i++) {
            fib[i] = fib[i-1] + fib[i-2];
        }

        for (int num : fib) {
            System.out.print(num + " ");
        }

        // Versão sem array (mais eficiente em memória)
        System.out.println("\n\nVersão otimizada:");
        int a = 0, b = 1;
        System.out.print(a + " " + b + " ");

        for (int i = 2; i < n; i++) {
            int c = a + b;
            System.out.print(c + " ");
            a = b;
            b = c;
        }
    }
}
```

**Desafio 3: Calculadora de Juros Compostos**

```java
public class JurosCompostos {
    public static void main(String[] args) {
        double principal = 1000.0; // Valor inicial
        double taxaAnual = 0.05; // 5% ao ano
        int anos = 10;

        System.out.println("Investimento inicial: R$ " + principal);
        System.out.println("Taxa anual: " + (taxaAnual * 100) + "%");
        System.out.println("Período: " + anos + " anos\n");

        System.out.println("Ano | Valor Acumulado");
        System.out.println("----|----------------");

        for (int ano = 1; ano <= anos; ano++) {
            double montante = principal * Math.pow(1 + taxaAnual, ano);
            System.out.printf("%3d | R$ %10.2f%n", ano, montante);
        }

        // Cálculo com aportes mensais
        System.out.println("\n=== COM APORTES MENSÁIS ===");
        double aporteMensal = 100.0;
        double taxaMensal = taxaAnual / 12;
        double total = principal;

        System.out.println("Aporte mensal: R$ " + aporteMensal);
        System.out.println("\nMês | Valor Acumulado");
        System.out.println("----|----------------");

        for (int mes = 1; mes <= anos * 12; mes++) {
            total = total * (1 + taxaMensal) + aporteMensal;
            if (mes % 12 == 0) {
                System.out.printf("%3d | R$ %10.2f%n", mes / 12, total);
            }
        }
    }
}
```

## **3.8 Material de Apoio**

**Resumo das Estruturas de Controle:**

**Condicionais:**
- `if-else`: Controle de fluxo baseado em condições booleanas
- `switch`: Seleção baseada em valores discretos

**Loops:**
- `for`: Número conhecido de iterações
- `while`: Condição de parada baseada em expressão booleana
- `do-while`: Executa pelo menos uma vez
- `for-each`: Iteração simplificada sobre coleções

**Controle de Fluxo:**
- `break`: Sai do loop ou switch
- `continue`: Pula para próxima iteração do loop
- `return`: Sai do método
- `labels`: Controle de loops aninhados

**Arrays:**
- Coleção de elementos do mesmo tipo
- Índice baseado em 0
- Tamanho fixo após criação

**Dicas Importantes:**
- Prefira `switch expressions` sobre `switch statements` quando possível
- Use `break` em switch statements para evitar fall-through não intencional
- Evite loops infinitos acidentais garantindo que a condição de parada seja alcançada
- Use enhanced for quando não precisar do índice
- Arrays.copyOf() é útil para criar cópias de arrays

---

**Próximo Módulo: Programação Orientada a Objetos**

Preparado para mergulhar nos conceitos fundamentais de OOP? O próximo módulo cobrirá classes, objetos, herança, polimorfismo e muito mais!

---

# **Módulo 4: Programação Orientada a Objetos**

## **4.1 Objetivos do Módulo**

- Compreender os pilares da OOP: encapsulamento, herança, polimorfismo e abstração
- Dominar a criação de classes, objetos, construtores e métodos
- Aprender a usar herança e composição
- Entender interfaces e classes abstratas
- Trabalhar com enums, records e sealed classes

## **4.2 Conteúdo Programático**

### **4.2.1 Classes e Objetos**

**Exemplo 4.1: Classe com Construtores e Métodos**

```java
public class Carro {
    // Campos (atributos)
    private String marca;
    private String modelo;
    private int ano;
    private double velocidade;

    // Construtor padrão
    public Carro() {
        this.marca = "Desconhecida";
        this.modelo = "Desconhecido";
        this.ano = 2020;
        this.velocidade = 0;
    }

    // Construtor parametrizado
    public Carro(String marca, String modelo, int ano) {
        this.marca = marca;
        this.modelo = modelo;
        this.ano = ano;
        this.velocidade = 0;
    }

    // Métodos de instância
    public void acelerar(double incremento) {
        if (incremento > 0) {
            this.velocidade += incremento;
            System.out.println("Acelerando para " + this.velocidade + " km/h");
        }
    }

    public void frear(double decremento) {
        if (decremento > 0) {
            this.velocidade = Math.max(0, this.velocidade - decremento);
            System.out.println("Reduzindo para " + this.velocidade + " km/h");
        }
    }

    // Métodos de acesso (Getters e Setters)
    public String getMarca() {
        return marca;
    }

    public void setMarca(String marca) {
        this.marca = marca;
    }

    public String getModelo() {
        return modelo;
    }

    public void setModelo(String modelo) {
        this.modelo = modelo;
    }

    public int getAno() {
        return ano;
    }

    public void setAno(int ano) {
        this.ano = ano;
    }

    public double getVelocidade() {
        return velocidade;
    }

    // Método toString
    @Override
    public String toString() {
        return String.format("Carro: %s %s (%d) - Velocidade: %.1f km/h",
                marca, modelo, ano, velocidade);
    }

    // Método equals
    @Override
    public boolean equals(Object obj) {
        if (this == obj) return true;
        if (obj == null || getClass() != obj.getClass()) return false;
        Carro carro = (Carro) obj;
        return ano == carro.ano &&
                Objects.equals(marca, carro.marca) &&
                Objects.equals(modelo, carro.modelo);
    }

    // Método hashCode
    @Override
    public int hashCode() {
        return Objects.hash(marca, modelo, ano);
    }
}

// Classe de teste
public class TesteCarro {
    public static void main(String[] args) {
        Carro carro1 = new Carro();
        Carro carro2 = new Carro("Toyota", "Corolla", 2022);

        carro1.setMarca("Honda");
        carro1.setModelo("Civic");
        carro1.setAno(2021);

        carro1.acelerar(50);
        carro2.acelerar(30);

        System.out.println(carro1);
        System.out.println(carro2);

        System.out.println("carro1 equals carro2? " + carro1.equals(carro2));
    }
}
```

### **4.2.2 Herança**

**Exemplo 4.2: Herança e Polimorfismo**

```java
// Superclasse
public class Veiculo {
    protected String marca;
    protected String modelo;
    protected int ano;

    public Veiculo(String marca, String modelo, int ano) {
        this.marca = marca;
        this.modelo = modelo;
        this.ano = ano;
    }

    public void mover() {
        System.out.println("O veículo está se movendo");
    }

    public void exibirInfo() {
        System.out.printf("Marca: %s, Modelo: %s, Ano: %d%n", marca, modelo, ano);
    }

    // Getters e Setters
    public String getMarca() { return marca; }
    public void setMarca(String marca) { this.marca = marca; }
    public String getModelo() { return modelo; }
    public void setModelo(String modelo) { this.modelo = modelo; }
    public int getAno() { return ano; }
    public void setAno(int ano) { this.ano = ano; }
}

// Subclasse Carro
public class Carro extends Veiculo {
    private int numeroPortas;

    public Carro(String marca, String modelo, int ano, int numeroPortas) {
        super(marca, modelo, ano); // Chamada ao construtor da superclasse
        this.numeroPortas = numeroPortas;
    }

    @Override
    public void mover() {
        System.out.println("O carro " + marca + " " + modelo + " está andando na estrada");
    }

    public void abrirPortas() {
        System.out.println("Abrindo " + numeroPortas + " portas");
    }

    @Override
    public void exibirInfo() {
        super.exibirInfo();
        System.out.println("Número de portas: " + numeroPortas);
    }

    public int getNumeroPortas() { return numeroPortas; }
    public void setNumeroPortas(int numeroPortas) { this.numeroPortas = numeroPortas; }
}

// Subclasse Moto
public class Moto extends Veiculo {
    private int cilindradas;

    public Moto(String marca, String modelo, int ano, int cilindradas) {
        super(marca, modelo, ano);
        this.cilindradas = cilindradas;
    }

    @Override
    public void mover() {
        System.out.println("A moto " + marca + " " + modelo + " está correndo");
    }

    public void empinar() {
        System.out.println("A moto está empinando!");
    }

    @Override
    public void exibirInfo() {
        super.exibirInfo();
        System.out.println("Cilindradas: " + cilindradas);
    }

    public int getCilindradas() { return cilindradas; }
    public void setCilindradas(int cilindradas) { this.cilindradas = cilindradas; }
}

// Classe de teste
public class TesteVeiculos {
    public static void main(String[] args) {
        Veiculo[] veiculos = {
            new Carro("Toyota", "Corolla", 2022, 4),
            new Moto("Honda", "CB500", 2021, 500),
            new Carro("Ford", "Mustang", 2020, 2)
        };

        // Polimorfismo: chamada do método mover() específico de cada classe
        for (Veiculo v : veiculos) {
            v.mover();
            v.exibirInfo();
            System.out.println();
        }

        // Downcasting e uso de métodos específicos
        for (Veiculo v : veiculos) {
            if (v instanceof Carro) {
                Carro carro = (Carro) v;
                carro.abrirPortas();
            } else if (v instanceof Moto) {
                Moto moto = (Moto) v;
                moto.empinar();
            }
        }
    }
}
```

### **4.2.3 Modificadores de Acesso e Encapsulamento**

**Exemplo 4.3: Encapsulamento**

```java
public class ContaBancaria {
    // Campos privados (encapsulados)
    private String numeroConta;
    private String titular;
    private double saldo;
    private static int totalContas = 0;

    public ContaBancaria(String titular, double depositoInicial) {
        this.numeroConta = gerarNumeroConta();
        this.titular = titular;
        this.saldo = depositoInicial;
        totalContas++;
    }

    private String gerarNumeroConta() {
        return "CONTA-" + (1000 + totalContas);
    }

    // Métodos públicos para interagir com os dados encapsulados
    public void depositar(double valor) {
        if (valor > 0) {
            saldo += valor;
            System.out.printf("Depósito de R$ %.2f realizado. Saldo: R$ %.2f%n", valor, saldo);
        } else {
            System.out.println("Valor de depósito inválido");
        }
    }

    public boolean sacar(double valor) {
        if (valor > 0 && valor <= saldo) {
            saldo -= valor;
            System.out.printf("Saque de R$ %.2f realizado. Saldo: R$ %.2f%n", valor, saldo);
            return true;
        } else {
            System.out.println("Saldo insuficiente ou valor inválido");
            return false;
        }
    }

    public void transferir(ContaBancaria destino, double valor) {
        if (this.sacar(valor)) {
            destino.depositar(valor);
            System.out.printf("Transferência de R$ %.2f para %s realizada%n", valor, destino.titular);
        }
    }

    // Getters (acesso controlado)
    public String getNumeroConta() { return numeroConta; }
    public String getTitular() { return titular; }
    public double getSaldo() { return saldo; }
    public static int getTotalContas() { return totalContas; }

    // Setters com validação
    public void setTitular(String titular) {
        if (titular != null && !titular.trim().isEmpty()) {
            this.titular = titular;
        } else {
            System.out.println("Nome do titular inválido");
        }
    }

    @Override
    public String toString() {
        return String.format("Conta: %s, Titular: %s, Saldo: R$ %.2f", numeroConta, titular, saldo);
    }
}

// Teste
public class TesteConta {
    public static void main(String[] args) {
        ContaBancaria conta1 = new ContaBancaria("João Silva", 1000);
        ContaBancaria conta2 = new ContaBancaria("Maria Santos", 500);

        conta1.depositar(200);
        conta1.sacar(150);
        conta1.transferir(conta2, 300);

        System.out.println(conta1);
        System.out.println(conta2);
        System.out.println("Total de contas: " + ContaBancaria.getTotalContas());
    }
}
```

### **4.2.4 Classes Abstratas**

**Exemplo 4.4: Classes e Métodos Abstratos**

```java
// Classe abstrata - não pode ser instanciada
public abstract class Funcionario {
    protected String nome;
    protected String cpf;
    protected double salarioBase;

    public Funcionario(String nome, String cpf, double salarioBase) {
        this.nome = nome;
        this.cpf = cpf;
        this.salarioBase = salarioBase;
    }

    // Método abstrato - deve ser implementado pelas subclasses
    public abstract double calcularSalario();

    // Método concreto - já tem implementação
    public void exibirInfo() {
        System.out.printf("Nome: %s, CPF: %s, Salário Base: R$ %.2f%n",
                nome, cpf, salarioBase);
    }

    // Getters e Setters
    public String getNome() { return nome; }
    public void setNome(String nome) { this.nome = nome; }
    public String getCpf() { return cpf; }
    public void setCpf(String cpf) { this.cpf = cpf; }
    public double getSalarioBase() { return salarioBase; }
    public void setSalarioBase(double salarioBase) { this.salarioBase = salarioBase; }
}

// Subclasse concreta
public class Gerente extends Funcionario {
    private double bonus;

    public Gerente(String nome, String cpf, double salarioBase, double bonus) {
        super(nome, cpf, salarioBase);
        this.bonus = bonus;
    }

    @Override
    public double calcularSalario() {
        return salarioBase + bonus;
    }

    @Override
    public void exibirInfo() {
        super.exibirInfo();
        System.out.printf("Bônus: R$ %.2f, Salário Total: R$ %.2f%n",
                bonus, calcularSalario());
    }

    public double getBonus() { return bonus; }
    public void setBonus(double bonus) { this.bonus = bonus; }
}

// Outra subclasse concreta
public class Desenvolvedor extends Funcionario {
    private int horasExtras;
    private double valorHoraExtra;

    public Desenvolvedor(String nome, String cpf, double salarioBase,
                        int horasExtras, double valorHoraExtra) {
        super(nome, cpf, salarioBase);
        this.horasExtras = horasExtras;
        this.valorHoraExtra = valorHoraExtra;
    }

    @Override
    public double calcularSalario() {
        return salarioBase + (horasExtras * valorHoraExtra);
    }

    @Override
    public void exibirInfo() {
        super.exibirInfo();
        System.out.printf("Horas Extras: %d, Valor Hora Extra: R$ %.2f, Salário Total: R$ %.2f%n",
                horasExtras, valorHoraExtra, calcularSalario());
    }

    public int getHorasExtras() { return horasExtras; }
    public void setHorasExtras(int horasExtras) { this.horasExtras = horasExtras; }
    public double getValorHoraExtra() { return valorHoraExtra; }
    public void setValorHoraExtra(double valorHoraExtra) { this.valorHoraExtra = valorHoraExtra; }
}

// Teste
public class TesteFuncionarios {
    public static void main(String[] args) {
        Funcionario[] funcionarios = {
            new Gerente("Carlos Souza", "111.222.333-44", 8000, 2000),
            new Desenvolvedor("Ana Costa", "555.666.777-88", 5000, 10, 100)
        };

        for (Funcionario f : funcionarios) {
            f.exibirInfo();
            System.out.println();
        }

        // Não podemos instanciar uma classe abstrata
        // Funcionario f = new Funcionario("João", "123", 1000); // ERRO!
    }
}
```

### **4.2.5 Interfaces**

**Exemplo 4.5: Interfaces e Implementação Múltipla**

```java
// Interface para objetos que podem ser autenticados
public interface Autenticavel {
    boolean autenticar(String senha);
    void setSenha(String senha);
}

// Interface para objetos que podem ser exibidos
public interface Exibivel {
    void exibir();
    String getTipo();
}

// Classe que implementa múltiplas interfaces
public class Usuario implements Autenticavel, Exibivel {
    private String nome;
    private String email;
    private String senha;

    public Usuario(String nome, String email, String senha) {
        this.nome = nome;
        this.email = email;
        this.senha = senha;
    }

    // Implementação dos métodos da interface Autenticavel
    @Override
    public boolean autenticar(String senha) {
        return this.senha.equals(senha);
    }

    @Override
    public void setSenha(String senha) {
        this.senha = senha;
    }

    // Implementação dos métodos da interface Exibivel
    @Override
    public void exibir() {
        System.out.printf("Usuário: %s (%s)%n", nome, email);
    }

    @Override
    public String getTipo() {
        return "USUÁRIO";
    }

    // Getters e Setters
    public String getNome() { return nome; }
    public void setNome(String nome) { this.nome = nome; }
    public String getEmail() { return email; }
    public void setEmail(String email) { this.email = email; }
}

// Outra classe que implementa as interfaces
public class Sistema implements Autenticavel, Exibivel {
    private String nome;
    private String senha;
    private String versao;

    public Sistema(String nome, String senha, String versao) {
        this.nome = nome;
        this.senha = senha;
        this.versao = versao;
    }

    @Override
    public boolean autenticar(String senha) {
        return this.senha.equals(senha);
    }

    @Override
    public void setSenha(String senha) {
        this.senha = senha;
    }

    @Override
    public void exibir() {
        System.out.printf("Sistema: %s (Versão: %s)%n", nome, versao);
    }

    @Override
    public String getTipo() {
        return "SISTEMA";
    }

    public String getNome() { return nome; }
    public void setNome(String nome) { this.nome = nome; }
    public String getVersao() { return versao; }
    public void setVersao(String versao) { this.versao = versao; }
}

// Classe de teste
public class TesteInterfaces {
    public static void main(String[] args) {
        Autenticavel[] autenticaveis = {
            new Usuario("João", "joao@email.com", "123456"),
            new Sistema("ERP Corporativo", "admin123", "1.0.0")
        };

        Exibivel[] exibiveis = {
            new Usuario("Maria", "maria@email.com", "654321"),
            new Sistema("CRM", "crm456", "2.1.0")
        };

        // Testando autenticação
        System.out.println("=== AUTENTICAÇÃO ===");
        for (Autenticavel a : autenticaveis) {
            boolean autenticado = a.autenticar("123456");
            System.out.println("Autenticado: " + autenticado);
        }

        // Testando exibição
        System.out.println("\n=== EXIBIÇÃO ===");
        for (Exibivel e : exibiveis) {
            e.exibir();
            System.out.println("Tipo: " + e.getTipo());
        }

        // Usando instanceof
        System.out.println("\n=== INSTANCEOF ===");
        for (Autenticavel a : autenticaveis) {
            if (a instanceof Usuario) {
                Usuario u = (Usuario) a;
                System.out.println("É um usuário: " + u.getNome());
            } else if (a instanceof Sistema) {
                Sistema s = (Sistema) a;
                System.out.println("É um sistema: " + s.getNome());
            }
        }
    }
}
```

### **4.2.6 Enums**

**Exemplo 4.6: Enum com Construtores e Métodos**

```java
// Enum simples
public enum DiaSemana {
    SEGUNDA, TERCA, QUARTA, QUINTA, SEXTA, SABADO, DOMINGO
}

// Enum avançado com construtores e métodos
public enum StatusPedido {
    PENDENTE(1, "Pedido realizado"),
    PROCESSANDO(2, "Pedido em processamento"),
    ENVIADO(3, "Pedido enviado"),
    ENTREGUE(4, "Pedido entregue"),
    CANCELADO(0, "Pedido cancelado");

    private final int codigo;
    private final String descricao;

    // Construtor do enum (sempre privado)
    StatusPedido(int codigo, String descricao) {
        this.codigo = codigo;
        this.descricao = descricao;
    }

    // Métodos de acesso
    public int getCodigo() { return codigo; }
    public String getDescricao() { return descricao; }

    // Método para buscar enum por código
    public static StatusPedido porCodigo(int codigo) {
        for (StatusPedido status : values()) {
            if (status.codigo == codigo) {
                return status;
            }
        }
        throw new IllegalArgumentException("Código inválido: " + codigo);
    }

    // Método para verificar se é um status final
    public boolean isFinal() {
        return this == ENTREGUE || this == CANCELADO;
    }
}

// Classe usando enums
public class Pedido {
    private int numero;
    private StatusPedido status;

    public Pedido(int numero) {
        this.numero = numero;
        this.status = StatusPedido.PENDENTE;
    }

    public void avancarStatus() {
        switch (status) {
            case PENDENTE:
                status = StatusPedido.PROCESSANDO;
                break;
            case PROCESSANDO:
                status = StatusPedido.ENVIADO;
                break;
            case ENVIADO:
                status = StatusPedido.ENTREGUE;
                break;
            case ENTREGUE:
            case CANCELADO:
                System.out.println("Status final não pode ser avançado");
                break;
        }
    }

    public void cancelar() {
        if (!status.isFinal()) {
            status = StatusPedido.CANCELADO;
        } else {
            System.out.println("Pedido finalizado não pode ser cancelado");
        }
    }

    public void exibirStatus() {
        System.out.printf("Pedido #%d: %s (%s)%n",
                numero, status.getDescricao(), status);
    }

    // Getters e Setters
    public int getNumero() { return numero; }
    public StatusPedido getStatus() { return status; }
}

// Teste
public class TesteEnum {
    public static void main(String[] args) {
        // Enum simples
        DiaSemana hoje = DiaSemana.SEGUNDA;
        System.out.println("Hoje é: " + hoje);

        // Enum avançado
        Pedido pedido = new Pedido(123);
        pedido.exibirStatus();

        pedido.avancarStatus();
        pedido.exibirStatus();

        pedido.avancarStatus();
        pedido.exibirStatus();

        pedido.avancarStatus();
        pedido.exibirStatus();

        // Tentativa de avançar status final
        pedido.avancarStatus();

        // Testando métodos do enum
        System.out.println("\n=== TESTANDO ENUM ===");
        for (StatusPedido status : StatusPedido.values()) {
            System.out.printf("%s: %s (Código: %d, Final: %b)%n",
                    status, status.getDescricao(), status.getCodigo(), status.isFinal());
        }

        // Buscando por código
        StatusPedido status = StatusPedido.porCodigo(2);
        System.out.println("\nStatus com código 2: " + status);
    }
}
```

### **4.2.7 Records (Java 16+)**

**Exemplo 4.7: Records - Classes Imutáveis**

```java
// Record para representar um ponto 2D
public record Ponto(int x, int y) {
    // Construtor compacto (pode validar dados)
    public Ponto {
        if (x < 0 || y < 0) {
            throw new IllegalArgumentException("Coordenadas não podem ser negativas");
        }
    }

    // Método de instância
    public double distancia(Ponto outro) {
        int dx = x - outro.x;
        int dy = y - outro.y;
        return Math.sqrt(dx * dx + dy * dy);
    }

    // Método estático
    public static Ponto origem() {
        return new Ponto(0, 0);
    }
}

// Record para representar uma pessoa
public record Pessoa(String nome, int idade, String email) {
    // Construtor adicional
    public Pessoa(String nome, int idade) {
        this(nome, idade, null);
    }

    // Método de instância
    public boolean isAdulto() {
        return idade >= 18;
    }

    // Podemos sobrescrever métodos
    @Override
    public String toString() {
        return String.format("Pessoa[nome=%s, idade=%d, email=%s]", nome, idade, email);
    }
}

// Teste
public class TesteRecords {
    public static void main(String[] args) {
        // Criando records
        Ponto p1 = new Ponto(3, 4);
        Ponto p2 = new Ponto(0, 0);
        Ponto origem = Ponto.origem();

        Pessoa pessoa1 = new Pessoa("João", 25, "joao@email.com");
        Pessoa pessoa2 = new Pessoa("Maria", 17);

        // Usando métodos
        System.out.println("Distância: " + p1.distancia(p2));
        System.out.println("P1: " + p1);
        System.out.println("P2: " + p2);

        System.out.println("Pessoa1: " + pessoa1);
        System.out.println("Pessoa2: " + pessoa2);
        System.out.println("Pessoa1 é adulto? " + pessoa1.isAdulto());
        System.out.println("Pessoa2 é adulto? " + pessoa2.isAdulto());

        // Records têm equals, hashCode e toString automáticos
        Ponto p3 = new Ponto(3, 4);
        System.out.println("p1 equals p3? " + p1.equals(p3)); // true

        // Componentes são finais (imutáveis)
        System.out.println("Coordenadas de p1: (" + p1.x() + ", " + p1.y() + ")");
    }
}
```

### **4.2.8 Sealed Classes (Java 17+)**

**Exemplo 4.8: Sealed Classes e Interfaces**

```java
// Sealed interface - só permite as classes especificadas
public sealed interface Forma
    permits Circulo, Retangulo, Triangulo {

    double calcularArea();
    double calcularPerimetro();
}

// Classe final que implementa Forma
public final class Circulo implements Forma {
    private final double raio;

    public Circulo(double raio) {
        this.raio = raio;
    }

    @Override
    public double calcularArea() {
        return Math.PI * raio * raio;
    }

    @Override
    public double calcularPerimetro() {
        return 2 * Math.PI * raio;
    }

    public double getRaio() { return raio; }
}

// Classe não-sealed que implementa Forma
public non-sealed class Retangulo implements Forma {
    private final double largura;
    private final double altura;

    public Retangulo(double largura, double altura) {
        this.largura = largura;
        this.altura = altura;
    }

    @Override
    public double calcularArea() {
        return largura * altura;
    }

    @Override
    public double calcularPerimetro() {
        return 2 * (largura + altura);
    }

    public double getLargura() { return largura; }
    public double getAltura() { return altura; }
}

// Classe sealed que implementa Forma e tem suas próprias subclasses
public sealed class Triangulo implements Forma
    permits TrianguloEquilatero, TrianguloRetangulo {

    protected final double lado1, lado2, lado3;

    public Triangulo(double lado1, double lado2, double lado3) {
        this.lado1 = lado1;
        this.lado2 = lado2;
        this.lado3 = lado3;
    }

    @Override
    public double calcularArea() {
        // Fórmula de Heron
        double s = calcularPerimetro() / 2;
        return Math.sqrt(s * (s - lado1) * (s - lado2) * (s - lado3));
    }

    @Override
    public double calcularPerimetro() {
        return lado1 + lado2 + lado3;
    }

    public double getLado1() { return lado1; }
    public double getLado2() { return lado2; }
    public double getLado3() { return lado3; }
}

// Subclasse de Triangulo
public final class TrianguloEquilatero extends Triangulo {
    public TrianguloEquilatero(double lado) {
        super(lado, lado, lado);
    }

    @Override
    public double calcularArea() {
        return (Math.sqrt(3) / 4) * lado1 * lado1;
    }
}

// Outra subclasse de Triangulo
public final class TrianguloRetangulo extends Triangulo {
    public TrianguloRetangulo(double cateto1, double cateto2) {
        super(cateto1, cateto2, Math.sqrt(cateto1 * cateto1 + cateto2 * cateto2));
    }

    @Override
    public double calcularArea() {
        return (lado1 * lado2) / 2;
    }
}

// Teste
public class TesteSealedClasses {
    public static void main(String[] args) {
        Forma[] formas = {
            new Circulo(5.0),
            new Retangulo(4.0, 6.0),
            new TrianguloEquilatero(3.0),
            new TrianguloRetangulo(3.0, 4.0)
        };

        for (Forma forma : formas) {
            System.out.printf("%s: Área = %.2f, Perímetro = %.2f%n",
                    forma.getClass().getSimpleName(),
                    forma.calcularArea(),
                    forma.calcularPerimetro());
        }

        // Pattern matching com instanceof (Java 16+)
        System.out.println("\n=== PATTERN MATCHING ===");
        for (Forma forma : formas) {
            String descricao = switch (forma) {
                case Circulo c -> String.format("Círculo com raio %.1f", c.getRaio());
                case Retangulo r -> String.format("Retângulo %.1fx%.1f", r.getLargura(), r.getAltura());
                case TrianguloEquilatero t -> String.format("Triângulo equilátero com lados %.1f", t.getLado1());
                case TrianguloRetangulo t -> String.format("Triângulo retângulo com catetos %.1f e %.1f",
                        t.getLado1(), t.getLado2());
                default -> "Forma desconhecida";
            };
            System.out.println(descricao);
        }
    }
}
```

## **4.3 Exercícios Práticos**

### **Exercício 4.1: Sistema de Biblioteca**

```java
// Implemente um sistema de biblioteca com as seguintes classes:
// 1. Livro (title, author, ISBN, disponível)
// 2. Membro (name, memberId, lista de livros emprestados)
// 3. Biblioteca (lista de livros, lista de membros)

// Use herança para diferentes tipos de membros (Estudante, Professor)
// Use interfaces para comportamentos (Emprestavel, Reservavel)
// Use enums para status dos livros (DISPONIVEL, EMPRESTADO, RESERVADO)

public interface Emprestavel {
    boolean emprestar(Membro membro);
    boolean devolver();
    boolean isDisponivel();
}

public enum StatusLivro {
    DISPONIVEL, EMPRESTADO, RESERVADO, MANUTENCAO
}

public class Livro implements Emprestavel {
    private String titulo;
    private String autor;
    private String isbn;
    private StatusLivro status;
    private Membro membroEmprestimo;

    // Construtor e métodos aqui...
}

public abstract class Membro {
    protected String nome;
    protected String id;
    protected int limiteEmprestimos;

    // Métodos abstratos e concretos aqui...
}

public class Estudante extends Membro {
    // Implementação específica para estudantes
}

public class Professor extends Membro {
    // Implementação específica para professores
}

public class Biblioteca {
    private List<Livro> livros;
    private List<Membro> membros;

    // Métodos para gerenciar livros e membros
}
```

### **Exercício 4.2: Sistema de Pagamentos**

```java
// Implemente um sistema de pagamentos com:
// 1. Interface Pagamento com métodos processarPagamento(), estornarPagamento()
// 2. Classes concretas: CartaoCredito, PayPal, TransferenciaBancaria
// 3. Classe Pedido que pode processar diferentes tipos de pagamento

public interface Pagamento {
    boolean processarPagamento(double valor);
    boolean estornarPagamento(double valor);
    String getTipoPagamento();
}

public record InfoCartao(String numero, String nomeTitular, String dataValidade, String cvv) {}

public class CartaoCredito implements Pagamento {
    private InfoCartao infoCartao;

    // Implementação dos métodos
}

public class PayPal implements Pagamento {
    private String email;

    // Implementação dos métodos
}

public class Pedido {
    private String numero;
    private double valor;
    private Pagamento pagamento;

    public boolean processar() {
        return pagamento.processarPagamento(valor);
    }
}
```

## **4.4 Questionário de Revisão**

**Questão 1:** Qual a diferença entre classe abstrata e interface?
- A) Classe abstrata pode ter implementação, interface só define contrato
- B) São a mesma coisa
- C) Interface pode ser instanciada

**Questão 2:** O que é polimorfismo?
- A) Capacidade de um objeto se comportar como diferentes tipos
- B) Herança múltipla
- C) Encapsulamento de dados

**Questão 3:** Para que serve o modificador `final`?
- A) Impede herança ou sobrescrita
- B) Torna a classe abstrata
- C) Permite herança múltipla

**Questão 4:** O que são records em Java?
- A) Classes imutáveis para armazenar dados
- B) Tipo de enumeração
- C) Interfaces funcionais

**Questão 5:** Qual a vantagem de sealed classes?

## **4.5 Laboratório Prático**

**Projeto: Sistema de Gerenciamento de Veículos**

```java
// Implemente um sistema completo de gerenciamento de veículos com:
// 1. Hierarquia de veículos (Carro, Moto, Caminhao)
// 2. Interfaces para comportamentos (Manutencao, Seguro)
// 3. Enums para tipos de combustível, status de manutenção
// 4. Records para informações de proprietário
// 5. Sealed classes para categorias de veículos

// Use todos os conceitos aprendidos no módulo
```

## **4.6 Material de Apoio**

**Resumo dos Conceitos de OOP:**

**Encapsulamento:**
- Ocultar dados internos e fornecer interface controlada
- Usar modificadores de acesso (private, protected, public)
- Implementar getters e setters

**Herança:**
- Estender funcionalidades de classes existentes
- Reutilização de código
- Relação "é-um"

**Polimorfismo:**
- Um objeto pode ser tratado como múltiplos tipos
- Sobrescrita de métodos (@Override)
- Ligação tardia (late binding)

**Abstração:**
- Classes abstratas (abstract)
- Interfaces
- Definir contratos sem implementação

**Novos Recursos:**
- **Enums**: Conjunto fixo de constantes
- **Records**: Classes imutáveis de dados
- **Sealed Classes**: Controle de hierarquia de herança

**Dicas Importantes:**
- Prefira composição sobre herança quando possível
- Use `@Override` para clarificar intenção
- Records são ideais para DTOs e value objects
- Sealed classes oferecem controle de hierarquia em tempo de compilação

---

**Próximo Módulo: Controle de Acesso e Pacotes**

Preparado para aprender sobre organização de código em pacotes, modificadores de acesso e o sistema de módulos do Java?

---

# **Módulo 5: Controle de Acesso e Encapsulamento**

## **5.1 Objetivos do Módulo**

- Compreender os modificadores de acesso em Java
- Dominar a estrutura de pacotes e imports
- Aprender a criar e usar classes imutáveis
- Entender o princípio de encapsulamento
- Trabalhar com o sistema de módulos Java

## **5.2 Conteúdo Programático**

### **5.2.1 Modificadores de Acesso**

**Exemplo 5.1: Modificadores de Acesso em Ação**

```java
// Arquivo: exemplos/ModificadoresAcesso.java
package exemplos;

public class ModificadoresAcesso {
    // public - acessível de qualquer lugar
    public String publico = "Público";
    
    // protected - acessível no mesmo pacote e por subclasses
    protected String protegido = "Protegido";
    
    // default (package-private) - acessível apenas no mesmo pacote
    String pacote = "Pacote";
    
    // private - acessível apenas na própria classe
    private String privado = "Privado";
    
    // Métodos com diferentes níveis de acesso
    public void metodoPublico() {
        System.out.println("Método público");
        // Pode acessar todos os campos da própria classe
        System.out.println(privado);
    }
    
    protected void metodoProtegido() {
        System.out.println("Método protegido");
    }
    
    void metodoPacote() {
        System.out.println("Método de pacote");
    }
    
    private void metodoPrivado() {
        System.out.println("Método privado");
    }
    
    // Método público que usa método privado internamente
    public void operacaoComplexa() {
        validarDados(); // Método privado usado internamente
        System.out.println("Operação complexa realizada");
    }
    
    private void validarDados() {
        System.out.println("Validando dados internamente...");
    }
}

// Subclasse no mesmo pacote
class Subclasse extends ModificadoresAcesso {
    public void testarAcesso() {
        System.out.println(publico);        // OK - público
        System.out.println(protegido);      // OK - protegido (herança)
        System.out.println(pacote);         // OK - mesmo pacote
        // System.out.println(privado);     // ERRO - privado
        
        metodoPublico();                    // OK
        metodoProtegido();                  // OK
        metodoPacote();                     // OK
        // metodoPrivado();                 // ERRO
    }
}

// Classe no mesmo pacote (não subclasse)
class OutraClasseMesmoPacote {
    public void testarAcesso() {
        ModificadoresAcesso obj = new ModificadoresAcesso();
        
        System.out.println(obj.publico);    // OK
        System.out.println(obj.protegido);  // OK - mesmo pacote
        System.out.println(obj.pacote);     // OK - mesmo pacote
        // System.out.println(obj.privado); // ERRO
        
        obj.metodoPublico();                // OK
        obj.metodoProtegido();              // OK - mesmo pacote
        obj.metodoPacote();                 // OK
        // obj.metodoPrivado();             // ERRO
    }
}
```

### **5.2.2 Estrutura de Pacotes**

**Exemplo 5.2: Organização em Pacotes**

```java
// Arquivo: com/empresa/projeto/dominio/Usuario.java
package com.empresa.projeto.dominio;

import java.time.LocalDateTime;
import java.util.Objects;

public class Usuario {
    private String id;
    private String nome;
    private String email;
    private LocalDateTime dataCriacao;
    
    public Usuario(String nome, String email) {
        this.id = java.util.UUID.randomUUID().toString();
        this.nome = nome;
        this.email = email;
        this.dataCriacao = LocalDateTime.now();
    }
    
    // Getters públicos
    public String getId() { return id; }
    public String getNome() { return nome; }
    public String getEmail() { return email; }
    public LocalDateTime getDataCriacao() { return dataCriacao; }
    
    // Setters com validação
    public void setNome(String nome) {
        if (nome == null || nome.trim().isEmpty()) {
            throw new IllegalArgumentException("Nome não pode ser vazio");
        }
        this.nome = nome;
    }
    
    public void setEmail(String email) {
        if (email == null || !email.contains("@")) {
            throw new IllegalArgumentException("Email inválido");
        }
        this.email = email;
    }
    
    @Override
    public boolean equals(Object o) {
        if (this == o) return true;
        if (o == null || getClass() != o.getClass()) return false;
        Usuario usuario = (Usuario) o;
        return Objects.equals(id, usuario.id);
    }
    
    @Override
    public int hashCode() {
        return Objects.hash(id);
    }
    
    @Override
    public String toString() {
        return String.format("Usuario{id='%s', nome='%s', email='%s'}", 
                           id, nome, email);
    }
}

// Arquivo: com/empresa/projeto/servico/UsuarioServico.java
package com.empresa.projeto.servico;

import com.empresa.projeto.dominio.Usuario;
import java.util.ArrayList;
import java.util.List;
import java.util.Optional;

public class UsuarioServico {
    private List<Usuario> usuarios;
    
    public UsuarioServico() {
        this.usuarios = new ArrayList<>();
    }
    
    public Usuario criarUsuario(String nome, String email) {
        Usuario usuario = new Usuario(nome, email);
        usuarios.add(usuario);
        return usuario;
    }
    
    public Optional<Usuario> buscarPorId(String id) {
        return usuarios.stream()
                      .filter(u -> u.getId().equals(id))
                      .findFirst();
    }
    
    public Optional<Usuario> buscarPorEmail(String email) {
        return usuarios.stream()
                      .filter(u -> u.getEmail().equalsIgnoreCase(email))
                      .findFirst();
    }
    
    public List<Usuario> listarTodos() {
        return new ArrayList<>(usuarios); // Retorna cópia para proteger a lista original
    }
    
    public boolean removerUsuario(String id) {
        return usuarios.removeIf(u -> u.getId().equals(id));
    }
}

// Arquivo: com/empresa/projeto/util/Validador.java
package com.empresa.projeto.util;

public class Validador {
    // Métodos utilitários estáticos
    public static boolean validarEmail(String email) {
        return email != null && email.matches("^[\\w.-]+@[\\w.-]+\\.\\w+$");
    }
    
    public static boolean validarNome(String nome) {
        return nome != null && nome.matches("^[a-zA-ZÀ-ÿ\\s]{2,50}$");
    }
    
    public static boolean validarSenha(String senha) {
        return senha != null && senha.length() >= 8;
    }
    
    // Construtor privado para prevenir instanciação
    private Validador() {
        throw new AssertionError("Classe utilitária não deve ser instanciada");
    }
}

// Arquivo: Principal.java (pacote padrão)
import com.empresa.projeto.dominio.Usuario;
import com.empresa.projeto.servico.UsuarioServico;
import com.empresa.projeto.util.Validador;

public class Principal {
    public static void main(String[] args) {
        UsuarioServico servico = new UsuarioServico();
        
        // Criar usuários
        Usuario usuario1 = servico.criarUsuario("João Silva", "joao@empresa.com");
        Usuario usuario2 = servico.criarUsuario("Maria Santos", "maria@empresa.com");
        
        // Buscar usuário
        servico.buscarPorId(usuario1.getId())
              .ifPresent(u -> System.out.println("Encontrado: " + u));
        
        // Listar todos
        System.out.println("\nTodos os usuários:");
        servico.listarTodos().forEach(System.out::println);
        
        // Validar dados
        System.out.println("\nValidações:");
        System.out.println("Email válido: " + Validador.validarEmail("teste@email.com"));
        System.out.println("Nome válido: " + Validador.validarNome("Ana"));
        System.out.println("Senha válida: " + Validador.validarSenha("12345678"));
    }
}
```

### **5.2.3 Classes Imutáveis**

**Exemplo 5.3: Implementando Classes Imutáveis**

```java
import java.util.*;

// Classe imutável - versão tradicional
public final class PessoaImutavel {
    private final String nome;
    private final int idade;
    private final List<String> telefones;
    private final Endereco endereco;
    
    public PessoaImutavel(String nome, int idade, List<String> telefones, Endereco endereco) {
        this.nome = Objects.requireNonNull(nome, "Nome não pode ser nulo");
        this.idade = idade;
        
        // Defensiva copy para a lista
        this.telefones = new ArrayList<>(Objects.requireNonNull(telefones));
        
        // Defensiva copy para o objeto mutável
        this.endereco = new Endereco(endereco.getRua(), endereco.getCidade());
    }
    
    // Getters
    public String getNome() { return nome; }
    public int getIdade() { return idade; }
    
    // Retorna cópia defensiva da lista
    public List<String> getTelefones() {
        return new ArrayList<>(telefones);
    }
    
    // Retorna cópia defensiva do objeto mutável
    public Endereco getEndereco() {
        return new Endereco(endereco.getRua(), endereco.getCidade());
    }
    
    // Método "with" para criar nova instância com modificações
    public PessoaImutavel withNome(String novoNome) {
        return new PessoaImutavel(novoNome, idade, telefones, endereco);
    }
    
    public PessoaImutavel withIdade(int novaIdade) {
        return new PessoaImutavel(nome, novaIdade, telefones, endereco);
    }
    
    @Override
    public boolean equals(Object o) {
        if (this == o) return true;
        if (o == null || getClass() != o.getClass()) return false;
        PessoaImutavel that = (PessoaImutavel) o;
        return idade == that.idade && 
               Objects.equals(nome, that.nome) && 
               Objects.equals(telefones, that.telefones) && 
               Objects.equals(endereco, that.endereco);
    }
    
    @Override
    public int hashCode() {
        return Objects.hash(nome, idade, telefones, endereco);
    }
    
    @Override
    public String toString() {
        return String.format("PessoaImutavel{nome='%s', idade=%d, telefones=%s, endereco=%s}",
                           nome, idade, telefones, endereco);
    }
}

// Classe mutável que será encapsulada
class Endereco {
    private String rua;
    private String cidade;
    
    public Endereco(String rua, String cidade) {
        this.rua = rua;
        this.cidade = cidade;
    }
    
    public String getRua() { return rua; }
    public String getCidade() { return cidade; }
    
    public void setRua(String rua) { this.rua = rua; }
    public void setCidade(String cidade) { this.cidade = cidade; }
    
    @Override
    public boolean equals(Object o) {
        if (this == o) return true;
        if (o == null || getClass() != o.getClass()) return false;
        Endereco endereco = (Endereco) o;
        return Objects.equals(rua, endereco.rua) && 
               Objects.equals(cidade, endereco.cidade);
    }
    
    @Override
    public int hashCode() {
        return Objects.hash(rua, cidade);
    }
    
    @Override
    public String toString() {
        return String.format("Endereco{rua='%s', cidade='%s'}", rua, cidade);
    }
}

// Record imutável (Java 16+)
record Produto(String nome, double preco, int quantidade) {
    // Construtor compacto para validação
    public Produto {
        if (nome == null || nome.trim().isEmpty()) {
            throw new IllegalArgumentException("Nome não pode ser vazio");
        }
        if (preco < 0) {
            throw new IllegalArgumentException("Preço não pode ser negativo");
        }
        if (quantidade < 0) {
            throw new IllegalArgumentException("Quantidade não pode ser negativa");
        }
    }
    
    // Método de instância
    public double calcularValorTotal() {
        return preco * quantidade;
    }
    
    // Método "with" para criar nova instância
    public Produto withPreco(double novoPreco) {
        return new Produto(nome, novoPreco, quantidade);
    }
    
    public Produto withQuantidade(int novaQuantidade) {
        return new Produto(nome, preco, novaQuantidade);
    }
}

// Classe de teste
public class TesteImutabilidade {
    public static void main(String[] args) {
        // Teste da classe imutável tradicional
        List<String> telefones = new ArrayList<>(Arrays.asList("1111-1111", "2222-2222"));
        Endereco endereco = new Endereco("Rua A", "São Paulo");
        
        PessoaImutavel pessoa = new PessoaImutavel("João", 30, telefones, endereco);
        
        // Tentativa de modificar a lista original (não afeta o objeto imutável)
        telefones.add("3333-3333");
        
        // Tentativa de modificar o endereço original (não afeta o objeto imutável)
        endereco.setRua("Rua B");
        
        System.out.println("Pessoa imutável: " + pessoa);
        System.out.println("Lista original modificada: " + telefones);
        System.out.println("Endereço original modificado: " + endereco);
        
        // Criando nova instância com modificação
        PessoaImutavel pessoaNova = pessoa.withIdade(31);
        System.out.println("Nova pessoa: " + pessoaNova);
        
        // Teste do record
        Produto produto = new Produto("Notebook", 2500.0, 2);
        System.out.println("\nProduto: " + produto);
        System.out.println("Valor total: " + produto.calcularValorTotal());
        
        Produto produtoComDesconto = produto.withPreco(2000.0);
        System.out.println("Produto com desconto: " + produtoComDesconto);
        
        // Tentativa de criar produto inválido
        try {
            Produto produtoInvalido = new Produto("", -100, -1);
        } catch (IllegalArgumentException e) {
            System.out.println("Erro esperado: " + e.getMessage());
        }
    }
}
```

### **5.2.4 Princípio de Encapsulamento**

**Exemplo 5.4: Encapsulamento em Prática**

```java
import java.util.*;

// Classe que demonstra encapsulamento adequado
public class ContaCorrente {
    private final String numero;
    private final String titular;
    private double saldo;
    private final double limite;
    private List<String> transacoes;
    private boolean ativa;
    
    public ContaCorrente(String numero, String titular, double limite) {
        this.numero = validarNumero(numero);
        this.titular = validarTitular(titular);
        this.limite = validarLimite(limite);
        this.saldo = 0.0;
        this.transacoes = new ArrayList<>();
        this.ativa = true;
        registrarTransacao("Conta criada");
    }
    
    // Validações privadas
    private String validarNumero(String numero) {
        if (numero == null || !numero.matches("\\d{4}-\\d{2}")) {
            throw new IllegalArgumentException("Número da conta inválido");
        }
        return numero;
    }
    
    private String validarTitular(String titular) {
        if (titular == null || titular.trim().length() < 3) {
            throw new IllegalArgumentException("Titular inválido");
        }
        return titular.trim();
    }
    
    private double validarLimite(double limite) {
        if (limite < 0) {
            throw new IllegalArgumentException("Limite não pode ser negativo");
        }
        return limite;
    }
    
    // Métodos públicos controlados
    public void depositar(double valor) {
        validarContaAtiva();
        if (valor <= 0) {
            throw new IllegalArgumentException("Valor de depósito deve ser positivo");
        }
        
        this.saldo += valor;
        registrarTransacao(String.format("Depósito: +R$ %.2f", valor));
    }
    
    public boolean sacar(double valor) {
        validarContaAtiva();
        if (valor <= 0) {
            throw new IllegalArgumentException("Valor de saque deve ser positivo");
        }
        
        if (valor <= saldo + limite) {
            this.saldo -= valor;
            registrarTransacao(String.format("Saque: -R$ %.2f", valor));
            return true;
        }
        
        registrarTransacao(String.format("Tentativa de saque recusada: R$ %.2f", valor));
        return false;
    }
    
    public boolean transferir(ContaCorrente destino, double valor) {
        validarContaAtiva();
        if (destino == null) {
            throw new IllegalArgumentException("Conta destino não pode ser nula");
        }
        
        if (this.sacar(valor)) {
            destino.depositar(valor);
            registrarTransacao(String.format("Transferência para %s: -R$ %.2f", 
                                           destino.numero, valor));
            return true;
        }
        return false;
    }
    
    public void desativarConta() {
        if (saldo != 0) {
            throw new IllegalStateException("Não é possível desativar conta com saldo não zero");
        }
        this.ativa = false;
        registrarTransacao("Conta desativada");
    }
    
    // Getters com informações controladas
    public String getNumero() { return numero; }
    public String getTitular() { return titular; }
    public double getSaldo() { return saldo; }
    public double getLimite() { return limite; }
    public boolean isAtiva() { return ativa; }
    
    // Getter que retorna cópia defensiva
    public List<String> getTransacoes() {
        return new ArrayList<>(transacoes);
    }
    
    // Método para obter extrato (não retorna a lista interna)
    public void imprimirExtrato() {
        System.out.println("\n=== EXTRATO DA CONTA " + numero + " ===");
        System.out.println("Titular: " + titular);
        System.out.println("Saldo: R$ " + String.format("%.2f", saldo));
        System.out.println("Limite: R$ " + String.format("%.2f", limite));
        System.out.println("Status: " + (ativa ? "Ativa" : "Inativa"));
        System.out.println("\nTransações:");
        transacoes.forEach(System.out::println);
    }
    
    // Métodos privados de apoio
    private void validarContaAtiva() {
        if (!ativa) {
            throw new IllegalStateException("Conta desativada");
        }
    }
    
    private void registrarTransacao(String descricao) {
        String timestamp = java.time.LocalDateTime.now().format(
            java.time.format.DateTimeFormatter.ofPattern("dd/MM/yyyy HH:mm:ss"));
        transacoes.add(timestamp + " - " + descricao);
    }
    
    @Override
    public String toString() {
        return String.format("ContaCorrente{numero='%s', titular='%s', saldo=%.2f, limite=%.2f, ativa=%s}",
                           numero, titular, saldo, limite, ativa);
    }
}

// Classe de teste
public class TesteEncapsulamento {
    public static void main(String[] args) {
        try {
            // Criar contas
            ContaCorrente conta1 = new ContaCorrente("1234-56", "João Silva", 1000.0);
            ContaCorrente conta2 = new ContaCorrente("7890-12", "Maria Santos", 500.0);
            
            // Operações
            conta1.depositar(2000.0);
            conta1.sacar(500.0);
            conta1.transferir(conta2, 300.0);
            
            // Tentar sacar valor acima do limite
            boolean saqueSucesso = conta1.sacar(3000.0);
            System.out.println("Saque de R$ 3000.00: " + (saqueSucesso ? "Sucesso" : "Falhou"));
            
            // Imprimir extratos
            conta1.imprimirExtrato();
            conta2.imprimirExtrato();
            
            // Tentar operações inválidas
            try {
                conta1.depositar(-100.0);
            } catch (IllegalArgumentException e) {
                System.out.println("\nErro esperado: " + e.getMessage());
            }
            
            // Tentar desativar conta com saldo
            try {
                conta1.desativarConta();
            } catch (IllegalStateException e) {
                System.out.println("Erro esperado: " + e.getMessage());
            }
            
        } catch (IllegalArgumentException e) {
            System.out.println("Erro na criação da conta: " + e.getMessage());
        }
    }
}
```

### **5.2.5 Sistema de Módulos Java**

**Exemplo 5.5: Introdução aos Módulos Java**

```java
// Estrutura de exemplo para módulos:

/*
projeto-app/
├── src/
│   ├── module-info.java
│   └── com/
│       └── empresa/
│           └── app/
│               ├── Main.java
│               └── servico/
│                   └── Servico.java
*/

// module-info.java
/*
module com.empresa.app {
    requires java.base;          // Implícito, mas pode ser explícito
    requires java.sql;           // Para acesso a banco de dados
    requires java.logging;       // Para logging
    
    // Exporta pacotes para outros módulos
    exports com.empresa.app.servico;
    
    // Permite reflexão (se necessário)
    opens com.empresa.app to java.base;
}
*/

// Servico.java
package com.empresa.app.servico;

import java.util.logging.Logger;

public class Servico {
    private static final Logger logger = Logger.getLogger(Servico.class.getName());
    
    public void executar() {
        logger.info("Serviço executando...");
        // Implementação do serviço
    }
}

// Main.java
package com.empresa.app;

import com.empresa.app.servico.Servico;

public class Main {
    public static void main(String[] args) {
        System.out.println("Aplicação modular iniciada!");
        
        Servico servico = new Servico();
        servico.executar();
    }
}
```

## **5.3 Exercícios Práticos**

### **Exercício 5.1: Sistema de Autenticação com Encapsulamento**

```java
// Implemente um sistema de autenticação com:
// 1. Classe Usuario com dados encapsulados
// 2. Classe ServicoAutenticacao com métodos protegidos
// 3. Validações adequadas
// 4. Registro de atividades

public class Usuario {
    private final String id;
    private String nome;
    private String email;
    private String senhaHash;
    private boolean ativo;
    private final java.time.LocalDateTime dataCriacao;
    
    // Construtor e métodos aqui...
}

public class ServicoAutenticacao {
    private java.util.Map<String, Usuario> usuarios;
    private java.util.List<String> logAtividades;
    
    // Métodos: registrarUsuario, autenticar, alterarSenha, etc.
}
```

### **Exercício 5.2: Biblioteca com Pacotes**

```java
// Crie uma estrutura de pacotes para uma biblioteca:
// - dominio: Livro, Autor, Membro
// - servico: ServicoEmprestimo, ServicoCatalogo
// - util: Validador, Formatador
// - repositorio: RepositorioLivros, RepositorioMembros

// Organize as classes em pacotes adequados com modificadores de acesso apropriados
```

## **5.4 Questionário de Revisão**

**Questão 1:** Qual modificador de acesso permite acesso apenas por subclasses?
- A) public
- B) protected
- C) private
- D) default (package-private)

**Questão 2:** O que é "defensive copy"?
- A) Fazer backup dos dados
- B) Criar cópia de objetos mutáveis para proteger o estado
- C) Copiar arquivos de configuração
- D) Fazer cópia de segurança do código

**Questão 3:** Qual a principal vantagem do encapsulamento?
- A) Melhor performance
- B) Controle sobre o acesso aos dados
- C) Código mais curto
- D) Herança múltipla

**Questão 4:** Para que serve o arquivo module-info.java?
- A) Configurar o banco de dados
- B) Definir dependências e exportações de módulos
- C) Configurar logging
- D) Definir interfaces gráficas

**Questão 5:** Por que classes imutáveis são thread-safe?

## **5.5 Laboratório Prático**

**Projeto: Sistema de Gerenciamento de Estoque**

```java
// Implemente um sistema de gerenciamento de estoque com:
// 1. Estrutura de pacotes organizada
// 2. Classes com encapsulamento adequado
// 3. Classes imutáveis onde apropriado
// 4. Validações e verificações de segurança
// 5. Sistema de logging de operações

// Use todos os conceitos aprendidos no módulo
```

## **5.6 Material de Apoio**

**Resumo dos Modificadores de Acesso:**

| Modificador | Classe | Pacote | Subclasse | Mundo |
|-------------|--------|--------|-----------|-------|
| public      | ✅     | ✅     | ✅        | ✅    |
| protected   | ✅     | ✅     | ✅        | ❌    |
| default     | ✅     | ✅     | ❌        | ❌    |
| private     | ✅     | ❌     | ❌        | ❌    |

**Princípios de Encapsulamento:**
- Mantenha campos privados
- Forneça getters públicos quando necessário
- Use setters com validação
- Faça "defensive copy" de objetos mutáveis
- Documente o contrato da classe

**Boas Práticas com Pacotes:**
- Use nomes de pacotes reversos do domínio
- Organize por funcionalidade, não por tipo
- Mantenha o acoplamento entre pacotes baixo
- Use imports específicos em vez de wildcards

**Classes Imutáveis:**
- Declare a classe como final
- Torne todos os campos final e privados
- Não forneça métodos modificadores
- Faça "defensive copy" em construtores e getters
- Para modificações, forneça métodos "with"

**Sistema de Módulos:**
- requires: declara dependências
- exports: expõe pacotes para outros módulos
- opens: permite reflexão
- provides/uses: para injeção de dependência

---

**Próximo Módulo: Tratamento de Exceções**

Preparado para aprender sobre tratamento robusto de erros e exceções em Java?

---

# **Módulo 7: Classes Selecionadas da API Java**

## **7.1 Objetivos do Módulo**

- Dominar a classe Object e seus métodos fundamentais
- Compreender a imutabilidade da classe String e o uso de StringBuilder
- Aprender sobre classes wrapper e autoboxing
- Conhecer classes utilitárias como Math, Random, Arrays e System
- Trabalhar com a classe Optional para evitar NullPointerException

## **7.2 Conteúdo Programático**

### **7.2.1 A Classe Object**

**Exemplo 7.1: Métodos Fundamentais da Classe Object**

```java
import java.util.Objects;

public class ExemploObject {

    static class Pessoa {
        private String nome;
        private int idade;
        private String cpf;

        public Pessoa(String nome, int idade, String cpf) {
            this.nome = nome;
            this.idade = idade;
            this.cpf = cpf;
        }

        // Implementação do equals
        @Override
        public boolean equals(Object obj) {
            if (this == obj) return true;
            if (obj == null || getClass() != obj.getClass()) return false;
            Pessoa pessoa = (Pessoa) obj;
            return idade == pessoa.idade &&
                    Objects.equals(nome, pessoa.nome) &&
                    Objects.equals(cpf, pessoa.cpf);
        }

        // Implementação do hashCode
        @Override
        public int hashCode() {
            return Objects.hash(nome, idade, cpf);
        }

        // Implementação do toString
        @Override
        public String toString() {
            return String.format("Pessoa{nome='%s', idade=%d, cpf='%s'}", nome, idade, cpf);
        }

        // Implementação do clone
        @Override
        public Pessoa clone() {
            try {
                return (Pessoa) super.clone();
            } catch (CloneNotSupportedException e) {
                throw new AssertionError(); // Não deve acontecer
            }
        }
    }

    public static void main(String[] args) {
        Pessoa p1 = new Pessoa("João", 25, "123.456.789-00");
        Pessoa p2 = new Pessoa("João", 25, "123.456.789-00");
        Pessoa p3 = new Pessoa("Maria", 30, "987.654.321-00");

        System.out.println("=== MÉTODOS OBJECT ===");

        // toString
        System.out.println("p1.toString(): " + p1.toString());
        System.out.println("p2: " + p2); // toString implícito

        // equals
        System.out.println("p1.equals(p2): " + p1.equals(p2)); // true
        System.out.println("p1.equals(p3): " + p1.equals(p3)); // false
        System.out.println("p1 == p2: " + (p1 == p2)); // false (referências diferentes)

        // hashCode
        System.out.println("p1.hashCode(): " + p1.hashCode());
        System.out.println("p2.hashCode(): " + p2.hashCode());
        System.out.println("p3.hashCode(): " + p3.hashCode());

        // getClass
        System.out.println("p1.getClass(): " + p1.getClass());
        System.out.println("Nome da classe: " + p1.getClass().getSimpleName());
        System.out.println("Nome completo: " + p1.getClass().getName());

        // clone
        Pessoa p4 = p1.clone();
        System.out.println("p1.clone(): " + p4);
        System.out.println("p1.equals(p4): " + p1.equals(p4)); // true

        // Métodos de sincronização (demonstração)
        System.out.println("\n=== SINCRONIZAÇÃO ===");
        Object lock = new Object();

        synchronized (lock) {
            System.out.println("Dentro do bloco sincronizado");
            try {
                lock.wait(100); // Espera por 100ms
            } catch (InterruptedException e) {
                e.printStackTrace();
            }
            lock.notify(); // Notifica uma thread em espera
        }
    }
}
```

### **7.2.2 Classes String e StringBuilder**

**Exemplo 7.2: Manipulação de Strings**

```java
public class ExemploString {

    public static void main(String[] args) {
        System.out.println("=== STRING (IMUTÁVEL) ===");

        // Criação de strings
        String str1 = "Java";
        String str2 = new String("Programming");
        String str3 = String.valueOf(123); // "123"
        String str4 = String.format("Nome: %s, Idade: %d", "João", 25);

        System.out.println("str1: " + str1);
        System.out.println("str2: " + str2);
        System.out.println("str3: " + str3);
        System.out.println("str4: " + str4);

        // Métodos principais
        String texto = " Java Programming Language ";

        System.out.println("\n=== MÉTODOS PRINCIPAIS ===");
        System.out.println("Original: '" + texto + "'");
        System.out.println("Comprimento: " + texto.length());
        System.out.println("Trim: '" + texto.trim() + "'");
        System.out.println("UpperCase: '" + texto.toUpperCase() + "'");
        System.out.println("LowerCase: '" + texto.toLowerCase() + "'");
        System.out.println("Substring(5, 16): '" + texto.substring(5, 16) + "'");
        System.out.println("Replace: '" + texto.replace("Java", "Python") + "'");
        System.out.println("Contains 'Programming': " + texto.contains("Programming"));
        System.out.println("StartsWith 'Java': " + texto.trim().startsWith("Java"));
        System.out.println("EndsWith 'Language': " + texto.trim().endsWith("Language"));
        System.out.println("IndexOf 'Prog': " + texto.indexOf("Prog"));
        System.out.println("LastIndexOf 'a': " + texto.lastIndexOf("a"));

        // Split e join
        String csv = "Java,Python,JavaScript,C++,Ruby";
        String[] linguagens = csv.split(",");
        System.out.println("\nSplit:");
        for (String lang : linguagens) {
            System.out.println(" - " + lang);
        }

        String joined = String.join(" | ", linguagens);
        System.out.println("Joined: " + joined);

        // Comparação
        String a = "java";
        String b = "JAVA";
        String c = "java";

        System.out.println("\n=== COMPARAÇÃO ===");
        System.out.println("a.equals(b): " + a.equals(b)); // false
        System.out.println("a.equalsIgnoreCase(b): " + a.equalsIgnoreCase(b)); // true
        System.out.println("a == c: " + (a == c)); // true (string pool)
        System.out.println("a.compareTo(b): " + a.compareTo(b)); // > 0
        System.out.println("a.compareToIgnoreCase(b): " + a.compareToIgnoreCase(b)); // 0

        // StringBuilder (Mutável)
        System.out.println("\n=== STRINGBUILDER (MUTÁVEL) ===");

        StringBuilder sb = new StringBuilder();
        sb.append("Java");
        sb.append(" ");
        sb.append("Programming");
        sb.append(" ");
        sb.append("Language");

        System.out.println("Conteúdo: " + sb.toString());
        System.out.println("Comprimento: " + sb.length());
        System.out.println("Capacidade: " + sb.capacity());

        // Inserção e modificação
        sb.insert(5, "Awesome ");
        System.out.println("Após inserção: " + sb);

        sb.replace(0, 4, "Python");
        System.out.println("Após replace: " + sb);

        sb.delete(6, 14);
        System.out.println("Após delete: " + sb);

        sb.reverse();
        System.out.println("Reverso: " + sb);
        sb.reverse(); // Volta ao normal

        // Comparação de performance
        System.out.println("\n=== PERFORMANCE ===");

        // Concatenação com String (ineficiente)
        long start = System.currentTimeMillis();
        String result = "";
        for (int i = 0; i < 10000; i++) {
            result += i; // Cria novo objeto a cada iteração
        }
        long end = System.currentTimeMillis();
        System.out.println("Tempo com String: " + (end - start) + "ms");

        // Concatenação com StringBuilder (eficiente)
        start = System.currentTimeMillis();
        StringBuilder sb2 = new StringBuilder();
        for (int i = 0; i < 10000; i++) {
            sb2.append(i); // Modifica o mesmo objeto
        }
        end = System.currentTimeMillis();
        System.out.println("Tempo com StringBuilder: " + (end - start) + "ms");
    }
}
```

### **7.2.3 Classes Wrapper e Autoboxing**

**Exemplo 7.3: Wrappers e Conversões**

```java
public class ExemploWrapper {

    public static void main(String[] args) {
        System.out.println("=== CLASSES WRAPPER ===");

        // Autoboxing: primitivo → wrapper (automático)
        Integer i = 100; // int → Integer
        Double d = 3.14; // double → Double
        Boolean b = true; // boolean → Boolean
        Character c = 'A'; // char → Character

        // Unboxing: wrapper → primitivo (automático)
        int iVal = i; // Integer → int
        double dVal = d; // Double → double
        boolean bVal = b; // Boolean → boolean
        char cVal = c; // Character → char

        System.out.println("Integer: " + i);
        System.out.println("Double: " + d);
        System.out.println("Boolean: " + b);
        System.out.println("Character: " + c);

        // Métodos úteis
        System.out.println("\n=== MÉTODOS ÚTEIS ===");
        System.out.println("Integer.MAX_VALUE: " + Integer.MAX_VALUE);
        System.out.println("Integer.MIN_VALUE: " + Integer.MIN_VALUE);
        System.out.println("Double.NaN: " + Double.NaN);
        System.out.println("Double.POSITIVE_INFINITY: " + Double.POSITIVE_INFINITY);
        System.out.println("Boolean.TRUE: " + Boolean.TRUE);

        // Parsing (String → primitivo/wrapper)
        System.out.println("\n=== PARSING ===");
        int num1 = Integer.parseInt("123");
        double num2 = Double.parseDouble("3.14");
        boolean flag = Boolean.parseBoolean("true");

        Integer num3 = Integer.valueOf("456");
        Double num4 = Double.valueOf("2.71");
        Boolean flag2 = Boolean.valueOf("false");

        System.out.println("parseInt: " + num1);
        System.out.println("parseDouble: " + num2);
        System.out.println("parseBoolean: " + flag);
        System.out.println("valueOf Integer: " + num3);
        System.out.println("valueOf Double: " + num4);
        System.out.println("valueOf Boolean: " + flag2);

        // Conversão para String
        System.out.println("\n=== CONVERSÃO PARA STRING ===");
        String s1 = Integer.toString(789);
        String s2 = Double.toString(1.618);
        String s3 = Boolean.toString(true);
        String s4 = String.valueOf(42); // Método genérico

        System.out.println("Integer.toString: " + s1);
        System.out.println("Double.toString: " + s2);
        System.out.println("Boolean.toString: " + s3);
        System.out.println("String.valueOf: " + s4);

        // Comparação de wrappers
        System.out.println("\n=== COMPARAÇÃO ===");
        Integer x = 100;
        Integer y = 100;
        Integer z = 200;
        Integer w = 200;

        System.out.println("x == y (cache -128 a 127): " + (x == y)); // true
        System.out.println("z == w (fora do cache): " + (z == w)); // false
        System.out.println("z.equals(w): " + z.equals(w)); // true

        // Métodos de conversão
        System.out.println("\n=== CONVERSÕES ===");
        System.out.println("Integer.toBinaryString(10): " + Integer.toBinaryString(10));
        System.out.println("Integer.toHexString(255): " + Integer.toHexString(255));
        System.out.println("Integer.toOctalString(64): " + Integer.toOctalString(64));

        // Operações matemáticas
        System.out.println("\n=== OPERAÇÕES MATEMÁTICAS ===");
        System.out.println("Integer.sum(10, 20): " + Integer.sum(10, 20));
        System.out.println("Integer.max(10, 20): " + Integer.max(10, 20));
        System.out.println("Integer.min(10, 20): " + Integer.min(10, 20));

        // Verificações
        System.out.println("\n=== VERIFICAÇÕES ===");
        System.out.println("Character.isDigit('5'): " + Character.isDigit('5'));
        System.out.println("Character.isLetter('A'): " + Character.isLetter('A'));
        System.out.println("Character.isWhitespace(' '): " + Character.isWhitespace(' '));
        System.out.println("Double.isNaN(Math.sqrt(-1)): " + Double.isNaN(Math.sqrt(-1)));
    }
}
```

### **7.2.4 Classes Utilitárias: Math, Random, Arrays**

**Exemplo 7.4: Classes Utilitárias**

```java
import java.util.Arrays;
import java.util.Random;
import java.util.concurrent.ThreadLocalRandom;

public class ExemploUtilitarias {

    public static void main(String[] args) {
        System.out.println("=== CLASSE MATH ===");

        // Constantes
        System.out.println("Math.PI: " + Math.PI);
        System.out.println("Math.E: " + Math.E);

        // Operações básicas
        System.out.println("Math.abs(-10): " + Math.abs(-10));
        System.out.println("Math.sqrt(25): " + Math.sqrt(25));
        System.out.println("Math.pow(2, 3): " + Math.pow(2, 3));
        System.out.println("Math.max(10, 20): " + Math.max(10, 20));
        System.out.println("Math.min(10, 20): " + Math.min(10, 20));

        // Arredondamento
        System.out.println("Math.round(3.14): " + Math.round(3.14));
        System.out.println("Math.ceil(3.14): " + Math.ceil(3.14));
        System.out.println("Math.floor(3.14): " + Math.floor(3.14));

        // Trigonometria
        System.out.println("Math.sin(Math.PI/2): " + Math.sin(Math.PI/2));
        System.out.println("Math.cos(0): " + Math.cos(0));
        System.out.println("Math.toDegrees(Math.PI): " + Math.toDegrees(Math.PI));

        // Logaritmos
        System.out.println("Math.log(10): " + Math.log(10));
        System.out.println("Math.log10(100): " + Math.log10(100));
        System.out.println("Math.exp(1): " + Math.exp(1));

        System.out.println("\n=== CLASSE RANDOM ===");

        Random random = new Random();

        System.out.println("random.nextInt(): " + random.nextInt());
        System.out.println("random.nextInt(100): " + random.nextInt(100));
        System.out.println("random.nextDouble(): " + random.nextDouble());
        System.out.println("random.nextBoolean(): " + random.nextBoolean());
        System.out.println("random.nextGaussian(): " + random.nextGaussian());

        // ThreadLocalRandom (Java 7+)
        System.out.println("ThreadLocalRandom.current().nextInt(1, 101): " +
                ThreadLocalRandom.current().nextInt(1, 101));

        System.out.println("\n=== CLASSE ARRAYS ===");

        int[] numeros = {5, 2, 8, 1, 9, 3};
        String[] nomes = {"João", "Maria", "Carlos", "Ana"};

        System.out.println("Array original: " + Arrays.toString(numeros));

        // Ordenação
        Arrays.sort(numeros);
        System.out.println("Array ordenado: " + Arrays.toString(numeros));

        Arrays.sort(nomes);
        System.out.println("Nomes ordenados: " + Arrays.toString(nomes));

        // Busca binária (array deve estar ordenado)
        int posicao = Arrays.binarySearch(numeros, 8);
        System.out.println("Posição do 8: " + posicao);

        // Preenchimento
        int[] arrayPreenchido = new int[5];
        Arrays.fill(arrayPreenchido, 42);
        System.out.println("Array preenchido: " + Arrays.toString(arrayPreenchido));

        // Cópia
        int[] copia = Arrays.copyOf(numeros, 3);
        System.out.println("Cópia parcial: " + Arrays.toString(copia));

        int[] copiaCompleta = Arrays.copyOf(numeros, numeros.length);
        System.out.println("Cópia completa: " + Arrays.toString(copiaCompleta));

        // Comparação
        System.out.println("Arrays.equals: " + Arrays.equals(numeros, copiaCompleta));

        // Array multidimensional
        int[][] matriz = {{1, 2, 3}, {4, 5, 6}, {7, 8, 9}};
        System.out.println("Matriz: " + Arrays.deepToString(matriz));

        System.out.println("\n=== CLASSE SYSTEM ===");

        // Propriedades do sistema
        System.out.println("Java version: " + System.getProperty("java.version"));
        System.out.println("OS: " + System.getProperty("os.name"));
        System.out.println("User: " + System.getProperty("user.name"));

        // Tempo
        long inicio = System.currentTimeMillis();
        long inicioNano = System.nanoTime();

        // Simular algum processamento
        try {
            Thread.sleep(100);
        } catch (InterruptedException e) {
            e.printStackTrace();
        }

        long fim = System.currentTimeMillis();
        long fimNano = System.nanoTime();

        System.out.println("Tempo decorrido (ms): " + (fim - inicio));
        System.out.println("Tempo decorrido (ns): " + (fimNano - inicioNano));

        // Variáveis de ambiente
        System.out.println("PATH: " + System.getenv("PATH"));

        // Saída de erro
        System.err.println("Esta é uma mensagem de erro!");
    }
}
```

### **7.2.5 A Classe Optional**

**Exemplo 7.5: Evitando NullPointerException com Optional**

```java
import java.util.Optional;

public class ExemploOptional {

    static class Usuario {
        private String nome;
        private String email;
        private Optional<String> telefone; // Campo opcional

        public Usuario(String nome, String email, String telefone) {
            this.nome = nome;
            this.email = email;
            this.telefone = Optional.ofNullable(telefone);
        }

        public String getNome() { return nome; }
        public String getEmail() { return email; }
        public Optional<String> getTelefone() { return telefone; }

        @Override
        public String toString() {
            return String.format("Usuario{nome='%s', email='%s', telefone=%s}",
                    nome, email, telefone.map(t -> "'" + t + "'").orElse("não informado"));
        }
    }

    public static void main(String[] args) {
        System.out.println("=== CLASSE OPTIONAL ===");

        // Criação de Optional
        Optional<String> optionalVazio = Optional.empty();
        Optional<String> optionalComValor = Optional.of("valor presente");
        Optional<String> optionalNulo = Optional.ofNullable(null);

        System.out.println("Optional vazio: " + optionalVazio);
        System.out.println("Optional com valor: " + optionalComValor);
        System.out.println("Optional nulo: " + optionalNulo);

        // Verificação de presença
        System.out.println("\n=== VERIFICAÇÃO ===");
        System.out.println("optionalVazio.isPresent(): " + optionalVazio.isPresent());
        System.out.println("optionalComValor.isPresent(): " + optionalComValor.isPresent());
        System.out.println("optionalVazio.isEmpty(): " + optionalVazio.isEmpty());

        // Obtenção de valores
        System.out.println("\n=== OBTENÇÃO DE VALORES ===");

        // get() - perigoso se vazio
        if (optionalComValor.isPresent()) {
            System.out.println("optionalComValor.get(): " + optionalComValor.get());
        }

        // orElse - valor padrão
        System.out.println("optionalVazio.orElse('valor padrão'): " +
                optionalVazio.orElse("valor padrão"));

        // orElseGet - supplier para valor padrão
        System.out.println("optionalVazio.orElseGet(() -> 'valor gerado'): " +
                optionalVazio.orElseGet(() -> "valor gerado"));

        // orElseThrow - lança exceção se vazio
        try {
            String valor = optionalVazio.orElseThrow(() ->
                    new RuntimeException("Valor não presente"));
        } catch (RuntimeException e) {
            System.out.println("Exceção capturada: " + e.getMessage());
        }

        // Transformações
        System.out.println("\n=== TRANSFORMAÇÕES ===");

        // map - transforma se presente
        Optional<Integer> tamanho = optionalComValor.map(String::length);
        System.out.println("Tamanho do valor: " + tamanho.orElse(0));

        // flatMap - para Optional aninhados
        Optional<Optional<String>> optionalAninhado = Optional.of(Optional.of("valor"));
        Optional<String> flat = optionalAninhado.flatMap(o -> o);
        System.out.println("FlatMap: " + flat);

        // filter - filtra valores
        Optional<String> filtrado = optionalComValor.filter(v -> v.length() > 10);
        System.out.println("Filtrado (length > 10): " + filtrado);

        // Ações condicionais
        System.out.println("\n=== AÇÕES CONDICIONAIS ===");

        // ifPresent - executa ação se presente
        optionalComValor.ifPresent(val -> System.out.println("Valor presente: " + val));
        optionalVazio.ifPresent(val -> System.out.println("Não será executado"));

        // ifPresentOrElse (Java 9+)
        optionalComValor.ifPresentOrElse(
                val -> System.out.println("Valor: " + val),
                () -> System.out.println("Valor ausente")
        );

        optionalVazio.ifPresentOrElse(
                val -> System.out.println("Não será executado"),
                () -> System.out.println("Valor está ausente")
        );

        // Caso de uso prático
        System.out.println("\n=== CASO PRÁTICO ===");

        Usuario usuario1 = new Usuario("João", "joao@email.com", "1234-5678");
        Usuario usuario2 = new Usuario("Maria", "maria@email.com", null);

        System.out.println("Usuário 1: " + usuario1);
        System.out.println("Usuário 2: " + usuario2);

        // Processamento seguro de telefone
        processarTelefone(usuario1);
        processarTelefone(usuario2);

        // Cadeia de métodos Optional
        String telefoneFormatado = usuario1.getTelefone()
                .map(t -> t.replace("-", ""))
                .map(t -> "(" + t.substring(0, 4) + ")" + t.substring(4))
                .orElse("Telefone não disponível");

        System.out.println("Telefone formatado: " + telefoneFormatado);
    }

    public static void processarTelefone(Usuario usuario) {
        usuario.getTelefone().ifPresentOrElse(
                telefone -> System.out.println("Enviando SMS para " + usuario.getNome() + ": " + telefone),
                () -> System.out.println("Usuário " + usuario.getNome() + " não tem telefone cadastrado")
        );
    }
}
```

## **7.3 Exercícios Práticos**

### **Exercício 7.1: Validador de CPF**

```java
public class ValidadorCPF {

    public static boolean validar(String cpf) {
        if (cpf == null) return false;

        // Remove caracteres não numéricos
        cpf = cpf.replaceAll("\\D", "");

        // Verifica tamanho
        if (cpf.length() != 11) return false;

        // Verifica se todos os dígitos são iguais
        if (cpf.matches("(\\d)\\1{10}")) return false;

        // Calcula primeiro dígito verificador
        int soma = 0;
        for (int i = 0; i < 9; i++) {
            soma += Character.getNumericValue(cpf.charAt(i)) * (10 - i);
        }
        int resto = soma % 11;
        int digito1 = (resto < 2) ? 0 : 11 - resto;

        // Verifica primeiro dígito
        if (digito1 != Character.getNumericValue(cpf.charAt(9))) {
            return false;
        }

        // Calcula segundo dígito verificador
        soma = 0;
        for (int i = 0; i < 10; i++) {
            soma += Character.getNumericValue(cpf.charAt(i)) * (11 - i);
        }
        resto = soma % 11;
        int digito2 = (resto < 2) ? 0 : 11 - resto;

        // Verifica segundo dígito
        return digito2 == Character.getNumericValue(cpf.charAt(10));
    }

    public static void main(String[] args) {
        String[] cpfs = {
            "123.456.789-09", // Válido (fictício)
            "111.444.777-35", // Válido
            "123.456.789-00", // Inválido
            "000.000.000-00", // Inválido
            "123" // Inválido
        };

        for (String cpf : cpfs) {
            System.out.printf("CPF %s é válido? %b%n", cpf, validar(cpf));
        }
    }
}
```

### **Exercício 7.2: Gerador de Senhas**

```java
import java.security.SecureRandom;
import java.util.Arrays;

public class GeradorSenhas {

    private static final String LETRAS_MAIUSCULAS = "ABCDEFGHIJKLMNOPQRSTUVWXYZ";
    private static final String LETRAS_MINUSCULAS = "abcdefghijklmnopqrstuvwxyz";
    private static final String NUMEROS = "0123456789";
    private static final String SIMBOLOS = "!@#$%^&*()_+-=[]{}|;:,.<>?";

    public static String gerarSenha(int comprimento, boolean usarMaiusculas,
                                   boolean usarMinusculas, boolean usarNumeros,
                                   boolean usarSimbolos) {

        if (comprimento < 4) {
            throw new IllegalArgumentException("Comprimento mínimo é 4");
        }

        StringBuilder caracteresPermitidos = new StringBuilder();
        if (usarMaiusculas) caracteresPermitidos.append(LETRAS_MAIUSCULAS);
        if (usarMinusculas) caracteresPermitidos.append(LETRAS_MINUSCULAS);
        if (usarNumeros) caracteresPermitidos.append(NUMEROS);
        if (usarSimbolos) caracteresPermitidos.append(SIMBOLOS);

        if (caracteresPermitidos.length() == 0) {
            throw new IllegalArgumentException("Pelo menos um tipo de caractere deve ser selecionado");
        }

        SecureRandom random = new SecureRandom();
        StringBuilder senha = new StringBuilder();

        // Garante pelo menos um de cada tipo selecionado
        if (usarMaiusculas) {
            senha.append(LETRAS_MAIUSCULAS.charAt(random.nextInt(LETRAS_MAIUSCULAS.length())));
        }
        if (usarMinusculas) {
            senha.append(LETRAS_MINUSCULAS.charAt(random.nextInt(LETRAS_MINUSCULAS.length())));
        }
        if (usarNumeros) {
            senha.append(NUMEROS.charAt(random.nextInt(NUMEROS.length())));
        }
        if (usarSimbolos) {
            senha.append(SIMBOLOS.charAt(random.nextInt(SIMBOLOS.length())));
        }

        // Preenche o restante
        while (senha.length() < comprimento) {
            senha.append(caracteresPermitidos.charAt(random.nextInt(caracteresPermitidos.length())));
        }

        // Embaralha a senha
        char[] senhaArray = senha.toString().toCharArray();
        for (int i = senhaArray.length - 1; i > 0; i--) {
            int j = random.nextInt(i + 1);
            char temp = senhaArray[i];
            senhaArray[i] = senhaArray[j];
            senhaArray[j] = temp;
        }

        return new String(senhaArray);
    }

    public static void main(String[] args) {
        System.out.println("=== GERADOR DE SENHAS ===");

        System.out.println("Senha simples: " + gerarSenha(8, true, true, true, false));
        System.out.println("Senha forte: " + gerarSenha(12, true, true, true, true));
        System.out.println("Senha numérica: " + gerarSenha(6, false, false, true, false));
        System.out.println("Senha com símbolos: " + gerarSenha(10, true, true, false, true));

        // Teste de força da senha
        String senhaForte = gerarSenha(16, true, true, true, true);
        System.out.println("Senha super forte: " + senhaForte);
        System.out.println("Comprimento: " + senhaForte.length());
        System.out.println("Contém maiúsculas: " + senhaForte.matches(".*[A-Z].*"));
        System.out.println("Contém minúsculas: " + senhaForte.matches(".*[a-z].*"));
        System.out.println("Contém números: " + senhaForte.matches(".*\\d.*"));
        System.out.println("Contém símbolos: " + senhaForte.matches(".*[!@#$%^&*()_+\\-=\\[\\]{}|;:,.<>?].*"));
    }
}
```

## **7.4 Caso Prático: Sistema de Análise de Texto**

```java
import java.util.*;
import java.util.stream.Collectors;

public class AnalisadorTexto {

    public static Map<String, Integer> contarPalavras(String texto) {
        if (texto == null || texto.trim().isEmpty()) {
            return Collections.emptyMap();
        }

        // Limpa e divide o texto em palavras
        String[] palavras = texto.toLowerCase()
                .replaceAll("[^a-záéíóúãõâêîôûàèìòùç\\s]", "")
                .split("\\s+");

        Map<String, Integer> contagem = new HashMap<>();

        for (String palavra : palavras) {
            if (!palavra.isEmpty()) {
                contagem.put(palavra, contagem.getOrDefault(palavra, 0) + 1);
            }
        }

        return contagem;
    }

    public static EstatisticasTexto analisarTexto(String texto) {
        if (texto == null) {
            return new EstatisticasTexto(0, 0, 0, 0, Collections.emptyMap());
        }

        int numeroCaracteres = texto.length();
        int numeroPalavras = texto.trim().isEmpty() ? 0 : texto.trim().split("\\s+").length;
        int numeroLinhas = texto.isEmpty() ? 0 : texto.split("\r\n|\r|\n").length;
        int numeroFrases = texto.split("[.!?]+").length;

        Map<String, Integer> palavrasFrequentes = contarPalavras(texto);

        return new EstatisticasTexto(
                numeroCaracteres, numeroPalavras, numeroLinhas, numeroFrases, palavrasFrequentes
        );
    }

    public static Optional<String> encontrarPalavraMaisFrequente(String texto) {
        Map<String, Integer> contagem = contarPalavras(texto);

        return contagem.entrySet().stream()
                .max(Map.Entry.comparingByValue())
                .map(Map.Entry::getKey);
    }

    public static List<String> encontrarPalavrasUnicas(String texto) {
        Map<String, Integer> contagem = contarPalavras(texto);

        return contagem.entrySet().stream()
                .filter(entry -> entry.getValue() == 1)
                .map(Map.Entry::getKey)
                .sorted()
                .collect(Collectors.toList());
    }

    static class EstatisticasTexto {
        private final int numeroCaracteres;
        private final int numeroPalavras;
        private final int numeroLinhas;
        private final int numeroFrases;
        private final Map<String, Integer> palavrasFrequentes;

        public EstatisticasTexto(int numeroCaracteres, int numeroPalavras,
                                int numeroLinhas, int numeroFrases,
                                Map<String, Integer> palavrasFrequentes) {
            this.numeroCaracteres = numeroCaracteres;
            this.numeroPalavras = numeroPalavras;
            this.numeroLinhas = numeroLinhas;
            this.numeroFrases = numeroFrases;
            this.palavrasFrequentes = palavrasFrequentes;
        }

        // Getters
        public int getNumeroCaracteres() { return numeroCaracteres; }
        public int getNumeroPalavras() { return numeroPalavras; }
        public int getNumeroLinhas() { return numeroLinhas; }
        public int getNumeroFrases() { return numeroFrases; }
        public Map<String, Integer> getPalavrasFrequentes() { return palavrasFrequentes; }

        @Override
        public String toString() {
            return String.format(
                    "EstatisticasTexto{caracteres=%d, palavras=%d, linhas=%d, frases=%d, palavrasUnicas=%d}",
                    numeroCaracteres, numeroPalavras, numeroLinhas, numeroFrases, palavrasFrequentes.size()
            );
        }
    }

    public static void main(String[] args) {
        String textoExemplo =
                "Java é uma linguagem de programação. Java é popular e poderosa. " +
                "Programação em Java é divertida. Java é usada em muitos projetos. " +
                "Aprender Java é importante para desenvolvedores.";

        System.out.println("=== ANÁLISE DE TEXTO ===");
        System.out.println("Texto: " + textoExemplo);

        EstatisticasTexto stats = analisarTexto(textoExemplo);
        System.out.println("\nEstatísticas: " + stats);

        System.out.println("\nContagem de palavras:");
        stats.getPalavrasFrequentes().entrySet().stream()
                .sorted(Map.Entry.<String, Integer>comparingByValue().reversed())
                .forEach(entry -> System.out.printf(" %s: %d%n", entry.getKey(), entry.getValue()));

        Optional<String> palavraMaisFrequente = encontrarPalavraMaisFrequente(textoExemplo);
        palavraMaisFrequente.ifPresent(palavra ->
                System.out.println("\nPalavra mais frequente: " + palavra)
        );

        List<String> palavrasUnicas = encontrarPalavrasUnicas(textoExemplo);
        System.out.println("\nPalavras únicas: " + palavrasUnicas);

        // Análise de texto vazio
        EstatisticasTexto statsVazio = analisarTexto("");
        System.out.println("\nEstatísticas texto vazio: " + statsVazio);
    }
}
```

## **7.5 Questionário de Revisão**

**Questão 1:** Qual a diferença entre String e StringBuilder?
- A) String é imutável, StringBuilder é mutável
- B) StringBuilder é mais lento para concatenação
- C) String é thread-safe, StringBuilder não é

**Questão 2:** O que é autoboxing em Java?
- A) Conversão automática de primitivo para wrapper
- B) Empacotamento de classes
- C) Conversão de String para número

**Questão 3:** Para que serve a classe Optional?
- A) Evitar NullPointerException
- B) Criar valores opcionais
- C) Ambas as anteriores

**Questão 4:** Qual método deve ser sobrescrito quando sobrescrever equals()?
- A) toString()
- B) hashCode()
- C) clone()

**Questão 5:** Qual a vantagem de ThreadLocalRandom sobre Random?
- A) Melhor performance em ambientes multi-thread
- B) Gera números mais aleatórios
- C) É mais fácil de usar

## **7.6 Laboratório Prático**

**Projeto: Biblioteca de Utilidades Matemáticas**

```java
// Implemente uma classe MathUtils que inclua:
// 1. Cálculo de números primos
// 2. Cálculo de fatorial
// 3. Conversão entre bases numéricas
// 4. Geração de sequências (Fibonacci, etc.)
// 5. Cálculos estatísticos (média, mediana, moda)

// Use todas as classes aprendidas: Math, Random, Arrays, Optional, etc.
```

## **7.7 Material de Apoio**

**Resumo das Classes Principais:**

**java.lang.Object:**
- `equals()` e `hashCode()`: Para comparação e uso em coleções
- `toString()`: Representação em string
- `clone()`: Cópia do objeto
- `getClass()`: Metadados da classe

**java.lang.String:**
- Imutável - operações retornam novas strings
- Métodos: `length()`, `substring()`, `replace()`, `split()`, etc.
- String pool - otimização de memória

**java.lang.StringBuilder:**
- Mutável - eficiente para concatenações
- Métodos: `append()`, `insert()`, `reverse()`, etc.

**Classes Wrapper:**
- `Integer`, `Double`, `Boolean`, `Character`
- Autoboxing/unboxing automático
- Métodos utilitários: `parseInt()`, `valueOf()`, etc.

**Classes Utilitárias:**
- `Math`: Operações matemáticas
- `Random`: Geração de números aleatórios
- `Arrays`: Manipulação de arrays
- `System`: Acesso ao sistema

**java.util.Optional:**
- Container para valores opcionais
- Evita `NullPointerException`
- Métodos: `of()`, `ofNullable()`, `map()`, `filter()`, etc.

**Dicas Importantes:**
- Use `StringBuilder` para concatenações em loops
- Sempre sobrescreva `hashCode()` quando sobrescrever `equals()`
- Use `Objects.equals()` para comparações seguras com null
- Prefira `ThreadLocalRandom` em ambientes multi-thread
- Use `Optional` para retornar valores que podem ser null

---

**Próximo Módulo: Coleções e Generics**

Preparado para explorar o framework de coleções do Java e o poder dos generics?

---

# **Módulo 8: Coleções e Generics**

## **8.1 Objetivos do Módulo**

- Compreender o framework de coleções do Java
- Dominar as principais interfaces: List, Set, Map, Queue
- Aprender a usar classes como ArrayList, HashSet, HashMap
- Entender o conceito de Generics e type safety
- Aprender a criar classes e métodos genéricos
- Trabalhar com Collections API e Streams (introdução)

## **8.2 Conteúdo Programático**

### **8.2.1 Introdução ao Framework de Coleções**

**Exemplo 8.1: Hierarquia de Coleções**

```java
import java.util.*;
import java.util.function.Consumer;

public class ExemploColecoes {

    public static void main(String[] args) {
        System.out.println("=== HIERARQUIA DE COLEÇÕES ===");

        // Collection vs Collections
        System.out.println("Collection: Interface raiz");
        System.out.println("Collections: Classe utilitária com métodos estáticos");

        // Principais interfaces
        System.out.println("\n=== INTERFACES PRINCIPAIS ===");
        System.out.println("List: Coleção ordenada, permite duplicatas");
        System.out.println("Set: Coleção não ordenada, não permite duplicatas");
        System.out.println("Map: Pares chave-valor, chaves únicas");
        System.out.println("Queue: Fila, ordem FIFO ou prioridade");

        // Demonstração básica
        demonstrarColecoes();
    }

    public static void demonstrarColecoes() {
        System.out.println("\n=== DEMONSTRAÇÃO PRÁTICA ===");

        // ArrayList (List)
        List<String> lista = new ArrayList<>();
        lista.add("Java");
        lista.add("Python");
        lista.add("JavaScript");
        lista.add("Java"); // Duplicata permitida

        System.out.println("Lista: " + lista);
        System.out.println("Tamanho: " + lista.size());
        System.out.println("Contém 'Java': " + lista.contains("Java"));
        System.out.println("Elemento na posição 1: " + lista.get(1));

        // HashSet (Set)
        Set<String> conjunto = new HashSet<>();
        conjunto.add("Apple");
        conjunto.add("Banana");
        conjunto.add("Orange");
        conjunto.add("Apple"); // Duplicata ignorada

        System.out.println("\nConjunto: " + conjunto);
        System.out.println("Tamanho: " + conjunto.size());
        System.out.println("Contém 'Banana': " + conjunto.contains("Banana"));

        // HashMap (Map)
        Map<String, Integer> mapa = new HashMap<>();
        mapa.put("João", 25);
        mapa.put("Maria", 30);
        mapa.put("Carlos", 28);
        mapa.put("João", 26); // Substitui valor anterior

        System.out.println("\nMapa: " + mapa);
        System.out.println("Tamanho: " + mapa.size());
        System.out.println("Idade do João: " + mapa.get("João"));
        System.out.println("Contém chave 'Maria': " + mapa.containsKey("Maria"));
        System.out.println("Contém valor 30: " + mapa.containsValue(30));

        // Iteração em coleções
        System.out.println("\n=== ITERAÇÃO ===");

        System.out.println("Iteração na Lista:");
        for (String elemento : lista) {
            System.out.println(" - " + elemento);
        }

        System.out.println("Iteração no Mapa:");
        for (Map.Entry<String, Integer> entry : mapa.entrySet()) {
            System.out.println(" - " + entry.getKey() + ": " + entry.getValue());
        }

        // Métodos utilitários da classe Collections
        System.out.println("\n=== COLLECTIONS UTIL ===");

        Collections.sort(lista);
        System.out.println("Lista ordenada: " + lista);

        Collections.reverse(lista);
        System.out.println("Lista reversa: " + lista);

        Collections.shuffle(lista);
        System.out.println("Lista embaralhada: " + lista);

        System.out.println("Máximo: " + Collections.max(lista));
        System.out.println("Mínimo: " + Collections.min(lista));
    }
}
```

### **8.2.2 List Interface e Implementações**

**Exemplo 8.2: Trabalhando com Lists**

```java
import java.util.*;

public class ExemploList {

    public static void main(String[] args) {
        System.out.println("=== LIST INTERFACE ===");

        // ArrayList vs LinkedList
        System.out.println("ArrayList: Acesso rápido por índice, inserções lentas no meio");
        System.out.println("LinkedList: Inserções rápidas, acesso lento por índice");

        // ArrayList
        List<String> arrayList = new ArrayList<>();
        arrayList.add("Elemento 1");
        arrayList.add("Elemento 2");
        arrayList.add("Elemento 3");
        arrayList.add(1, "Elemento 1.5"); // Inserção no meio

        System.out.println("\nArrayList: " + arrayList);
        System.out.println("Elemento no índice 2: " + arrayList.get(2));

        // LinkedList
        List<String> linkedList = new LinkedList<>();
        linkedList.add("Primeiro");
        linkedList.add("Segundo");
        linkedList.add("Terceiro");
        linkedList.addFirst("Zerésimo"); // Método específico LinkedList
        linkedList.addLast("Quarto");

        System.out.println("LinkedList: " + linkedList);
        System.out.println("Primeiro elemento: " + ((LinkedList<String>) linkedList).getFirst());
        System.out.println("Último elemento: " + ((LinkedList<String>) linkedList).getLast());

        // Vector (thread-safe, legado)
        List<String> vector = new Vector<>();
        vector.add("Item A");
        vector.add("Item B");
        vector.add("Item C");

        System.out.println("Vector: " + vector);

        // Operações comuns em List
        demonstrarOperacoesList();
    }

    public static void demonstrarOperacoesList() {
        System.out.println("\n=== OPERAÇÕES COM LIST ===");

        List<Integer> numeros = new ArrayList<>(Arrays.asList(1, 2, 3, 4, 5, 2, 3));

        System.out.println("Lista original: " + numeros);

        // Adição
        numeros.add(6);
        numeros.add(2, 99); // Insere na posição 2
        System.out.println("Após adições: " + numeros);

        // Remoção
        numeros.remove(1); // Remove pelo índice
        numeros.remove(Integer.valueOf(3)); // Remove pela primeira ocorrência do valor
        System.out.println("Após remoções: " + numeros);

        // Modificação
        numeros.set(0, 100);
        System.out.println("Após modificar índice 0: " + numeros);

        // Busca
        System.out.println("Índice do 4: " + numeros.indexOf(4));
        System.out.println("Último índice do 2: " + numeros.lastIndexOf(2));
        System.out.println("Contém 5: " + numeros.contains(5));

        // Sublista
        List<Integer> sublista = numeros.subList(1, 4);
        System.out.println("Sublista (1-4): " + sublista);

        // Conversão para array
        Integer[] array = numeros.toArray(new Integer[0]);
        System.out.println("Array: " + Arrays.toString(array));

        // Lista imutável (Java 9+)
        List<String> imutavel = List.of("A", "B", "C");
        System.out.println("Lista imutável: " + imutavel);

        // Tentativa de modificar lista imutável (lança exceção)
        try {
            imutavel.add("D");
        } catch (UnsupportedOperationException e) {
            System.out.println("Erro ao modificar lista imutável: " + e.getMessage());
        }
    }
}
```

### **8.2.3 Set Interface e Implementações**

**Exemplo 8.3: Trabalhando com Sets**

```java
import java.util.*;

public class ExemploSet {

    public static void main(String[] args) {
        System.out.println("=== SET INTERFACE ===");

        // HashSet vs TreeSet vs LinkedHashSet
        System.out.println("HashSet: Não ordenado, mais rápido");
        System.out.println("TreeSet: Ordenado naturalmente");
        System.out.println("LinkedHashSet: Mantém ordem de inserção");

        // HashSet
        Set<String> hashSet = new HashSet<>();
        hashSet.add("Maçã");
        hashSet.add("Banana");
        hashSet.add("Laranja");
        hashSet.add("Uva");
        hashSet.add("Banana"); // Duplicata ignorada

        System.out.println("\nHashSet: " + hashSet);
        System.out.println("Tamanho: " + hashSet.size());

        // TreeSet (ordenado)
        Set<String> treeSet = new TreeSet<>();
        treeSet.add("Zebra");
        treeSet.add("Abacaxi");
        treeSet.add("Cachorro");
        treeSet.add("Gato");

        System.out.println("TreeSet (ordenado): " + treeSet);

        // LinkedHashSet (ordem de inserção)
        Set<String> linkedHashSet = new LinkedHashSet<>();
        linkedHashSet.add("Primeiro");
        linkedHashSet.add("Segundo");
        linkedHashSet.add("Terceiro");
        linkedHashSet.add("Primeiro"); // Duplicata ignorada

        System.out.println("LinkedHashSet: " + linkedHashSet);

        // Operações com conjuntos
        demonstrarOperacoesConjuntos();
    }

    public static void demonstrarOperacoesConjuntos() {
        System.out.println("\n=== OPERAÇÕES COM CONJUNTOS ===");

        Set<Integer> conjuntoA = new HashSet<>(Arrays.asList(1, 2, 3, 4, 5));
        Set<Integer> conjuntoB = new HashSet<>(Arrays.asList(4, 5, 6, 7, 8));

        System.out.println("Conjunto A: " + conjuntoA);
        System.out.println("Conjunto B: " + conjuntoB);

        // União
        Set<Integer> uniao = new HashSet<>(conjuntoA);
        uniao.addAll(conjuntoB);
        System.out.println("União (A ∪ B): " + uniao);

        // Interseção
        Set<Integer> intersecao = new HashSet<>(conjuntoA);
        intersecao.retainAll(conjuntoB);
        System.out.println("Interseção (A ∩ B): " + intersecao);

        // Diferença
        Set<Integer> diferenca = new HashSet<>(conjuntoA);
        diferenca.removeAll(conjuntoB);
        System.out.println("Diferença (A - B): " + diferenca);

        // Diferença simétrica (união - interseção)
        Set<Integer> diferencaSimetrica = new HashSet<>(uniao);
        diferencaSimetrica.removeAll(intersecao);
        System.out.println("Diferença Simétrica (A Δ B): " + diferencaSimetrica);

        // Verificações
        System.out.println("A contém todos de B? " + conjuntoA.containsAll(conjuntoB));
        System.out.println("A é subconjunto de união? " + uniao.containsAll(conjuntoA));

        // Set com objetos customizados
        demonstrarSetCustom();
    }

    public static void demonstrarSetCustom() {
        System.out.println("\n=== SET COM OBJETOS CUSTOMIZADOS ===");

        class Produto {
            private String nome;
            private double preco;

            public Produto(String nome, double preco) {
                this.nome = nome;
                this.preco = preco;
            }

            // IMPORTANTE: Para usar em Set, deve-se sobrescrever equals() e hashCode()
            @Override
            public boolean equals(Object o) {
                if (this == o) return true;
                if (o == null || getClass() != o.getClass()) return false;
                Produto produto = (Produto) o;
                return Double.compare(produto.preco, preco) == 0 &&
                        Objects.equals(nome, produto.nome);
            }

            @Override
            public int hashCode() {
                return Objects.hash(nome, preco);
            }

            @Override
            public String toString() {
                return String.format("Produto{nome='%s', preco=%.2f}", nome, preco);
            }
        }

        Set<Produto> produtos = new HashSet<>();
        produtos.add(new Produto("Notebook", 2500.00));
        produtos.add(new Produto("Mouse", 50.00));
        produtos.add(new Produto("Teclado", 150.00));
        produtos.add(new Produto("Notebook", 2500.00)); // Duplicata (mesmo nome e preço)

        System.out.println("Produtos no conjunto: " + produtos.size());
        for (Produto p : produtos) {
            System.out.println(" - " + p);
        }
    }
}
```

### **8.2.4 Map Interface e Implementações**

**Exemplo 8.4: Trabalhando com Maps**

```java
import java.util.*;

public class ExemploMap {

    public static void main(String[] args) {
        System.out.println("=== MAP INTERFACE ===");

        // HashMap vs TreeMap vs LinkedHashMap
        System.out.println("HashMap: Não ordenado, mais rápido");
        System.out.println("TreeMap: Ordenado por chaves");
        System.out.println("LinkedHashMap: Mantém ordem de inserção");

        // HashMap
        Map<String, Integer> hashMap = new HashMap<>();
        hashMap.put("João", 25);
        hashMap.put("Maria", 30);
        hashMap.put("Carlos", 28);
        hashMap.put("Ana", 35);
        hashMap.put("João", 26); // Substitui valor anterior

        System.out.println("\nHashMap: " + hashMap);
        System.out.println("Idade de Maria: " + hashMap.get("Maria"));
        System.out.println("Contém chave 'Pedro'? " + hashMap.containsKey("Pedro"));

        // TreeMap (ordenado por chaves)
        Map<String, Integer> treeMap = new TreeMap<>();
        treeMap.put("Zebra", 100);
        treeMap.put("Abacate", 200);
        treeMap.put("Cachorro", 150);

        System.out.println("TreeMap (ordenado): " + treeMap);

        // LinkedHashMap (ordem de inserção)
        Map<String, Integer> linkedHashMap = new LinkedHashMap<>();
        linkedHashMap.put("Primeiro", 1);
        linkedHashMap.put("Segundo", 2);
        linkedHashMap.put("Terceiro", 3);

        System.out.println("LinkedHashMap: " + linkedHashMap);

        // Operações com mapas
        demonstrarOperacoesMap();
    }

    public static void demonstrarOperacoesMap() {
        System.out.println("\n=== OPERAÇÕES COM MAP ===");

        Map<String, List<String>> categorias = new HashMap<>();

        // Adicionando valores
        categorias.put("Frutas", Arrays.asList("Maçã", "Banana", "Laranja"));
        categorias.put("Verduras", Arrays.asList("Alface", "Couve", "Espinafre"));
        categorias.put("Legumes", Arrays.asList("Cenoura", "Batata", "Abobrinha"));

        System.out.println("Mapa de categorias: " + categorias);

        // Acessando valores
        System.out.println("Frutas: " + categorias.get("Frutas"));
        System.out.println("Chaves: " + categorias.keySet());
        System.out.println("Valores: " + categorias.values());

        // Métodos úteis
        System.out.println("Tamanho: " + categorias.size());
        System.out.println("Está vazio? " + categorias.isEmpty());
        System.out.println("Contém chave 'Carnes'? " + categorias.containsKey("Carnes"));

        // Iteração
        System.out.println("\n=== ITERAÇÃO NO MAPA ===");

        System.out.println("Por chave:");
        for (String chave : categorias.keySet()) {
            System.out.println(" - " + chave + ": " + categorias.get(chave));
        }

        System.out.println("Por entrada:");
        for (Map.Entry<String, List<String>> entrada : categorias.entrySet()) {
            System.out.println(" - " + entrada.getKey() + ": " + entrada.getValue());
        }

        System.out.println("Por valores:");
        for (List<String> valores : categorias.values()) {
            System.out.println(" - " + valores);
        }

        // Métodos de manipulação
        System.out.println("\n=== MANIPULAÇÃO AVANÇADA ===");

        // getOrDefault
        List<String> defaultList = Arrays.asList("Não categorizado");
        System.out.println("Carnes (com default): " + 
                categorias.getOrDefault("Carnes", defaultList));

        // putIfAbsent
        categorias.putIfAbsent("Frutas", Arrays.asList("Uva", "Manga"));
        System.out.println("Após putIfAbsent em Frutas: " + categorias.get("Frutas"));

        // computeIfAbsent
        categorias.computeIfAbsent("Bebidas", k -> new ArrayList<>())
                 .add("Água");
        System.out.println("Após computeIfAbsent Bebidas: " + categorias.get("Bebidas"));

        // merge
        Map<String, Integer> estoque = new HashMap<>();
        estoque.put("Maçã", 10);
        estoque.put("Banana", 5);
        
        estoque.merge("Maçã", 3, Integer::sum);
        estoque.merge("Laranja", 8, Integer::sum);
        
        System.out.println("Estoque após merge: " + estoque);

        // Map imutável
        Map<String, String> imutavel = Map.of(
            "chave1", "valor1",
            "chave2", "valor2",
            "chave3", "valor3"
        );
        System.out.println("Map imutável: " + imutavel);
    }
}
```

### **8.2.5 Queue Interface e Implementações**

**Exemplo 8.5: Trabalhando com Queues**

```java
import java.util.*;

public class ExemploQueue {

    public static void main(String[] args) {
        System.out.println("=== QUEUE INTERFACE ===");

        // LinkedList vs PriorityQueue
        System.out.println("LinkedList: Ordem FIFO");
        System.out.println("PriorityQueue: Ordem por prioridade");

        // Queue com LinkedList (FIFO)
        Queue<String> fila = new LinkedList<>();
        fila.offer("Primeiro"); // add() lança exceção se cheia, offer() retorna false
        fila.offer("Segundo");
        fila.offer("Terceiro");

        System.out.println("\nFila: " + fila);
        System.out.println("Próximo elemento: " + fila.peek()); // element() lança exceção

        // Processamento FIFO
        System.out.println("\nProcessamento FIFO:");
        while (!fila.isEmpty()) {
            System.out.println("Processando: " + fila.poll()); // remove() lança exceção
        }

        // PriorityQueue (ordem natural ou customizada)
        Queue<Integer> filaPrioridade = new PriorityQueue<>();
        filaPrioridade.offer(30);
        filaPrioridade.offer(10);
        filaPrioridade.offer(20);
        filaPrioridade.offer(5);

        System.out.println("\nPriorityQueue: " + filaPrioridade);
        
        System.out.println("Processamento por prioridade:");
        while (!filaPrioridade.isEmpty()) {
            System.out.println("Processando: " + filaPrioridade.poll());
        }

        // PriorityQueue com ordem customizada
        Queue<String> filaCustom = new PriorityQueue<>(
            Comparator.comparing(String::length).reversed()
        );
        
        filaCustom.offer("Curto");
        filaCustom.offer("Texto Médio");
        filaCustom.offer("Este é um texto longo");
        filaCustom.offer("Médio");

        System.out.println("\nPriorityQueue custom (maior length primeiro):");
        while (!filaCustom.isEmpty()) {
            System.out.println("Processando: " + filaCustom.poll());
        }

        // Deque (Double Ended Queue)
        demonstrarDeque();
    }

    public static void demonstrarDeque() {
        System.out.println("\n=== DEQUE INTERFACE ===");

        Deque<String> deque = new LinkedList<>();
        
        // Operações no início
        deque.addFirst("Primeiro");
        deque.offerFirst("Zerésimo");
        
        // Operações no final
        deque.addLast("Segundo");
        deque.offerLast("Terceiro");

        System.out.println("Deque: " + deque);
        System.out.println("Primeiro: " + deque.getFirst());
        System.out.println("Último: " + deque.getLast());

        // Remoção do início e final
        System.out.println("Removendo do início: " + deque.removeFirst());
        System.out.println("Removendo do final: " + deque.removeLast());
        
        System.out.println("Deque após remoções: " + deque);

        // Stack usando Deque (substitui Stack legado)
        Deque<String> stack = new ArrayDeque<>();
        stack.push("Elemento 1"); // push = addFirst
        stack.push("Elemento 2");
        stack.push("Elemento 3");

        System.out.println("\nStack (usando Deque): " + stack);
        System.out.println("Topo: " + stack.peek()); // peek = peekFirst
        
        while (!stack.isEmpty()) {
            System.out.println("Pop: " + stack.pop()); // pop = removeFirst
        }
    }
}
```

### **8.2.6 Introdução aos Generics**

**Exemplo 8.6: Fundamentos de Generics**

```java
import java.util.*;

public class ExemploGenerics {

    // Classe genérica
    static class Caixa<T> {
        private T conteudo;

        public void armazenar(T conteudo) {
            this.conteudo = conteudo;
        }

        public T obter() {
            return conteudo;
        }

        public boolean estaVazia() {
            return conteudo == null;
        }

        @Override
        public String toString() {
            return "Caixa{" + conteudo + "}";
        }
    }

    // Classe genérica com múltiplos tipos
    static class Par<K, V> {
        private K chave;
        private V valor;

        public Par(K chave, V valor) {
            this.chave = chave;
            this.valor = valor;
        }

        public K getChave() { return chave; }
        public V getValor() { return valor; }

        @Override
        public String toString() {
            return "Par{" + chave + "=" + valor + "}";
        }
    }

    // Método genérico
    public static <T> void imprimirArray(T[] array) {
        for (T elemento : array) {
            System.out.print(elemento + " ");
        }
        System.out.println();
    }

    // Método genérico com tipo limitado (bounded type)
    public static <T extends Comparable<T>> T encontrarMaximo(T[] array) {
        if (array == null || array.length == 0) {
            return null;
        }

        T maximo = array[0];
        for (T elemento : array) {
            if (elemento.compareTo(maximo) > 0) {
                maximo = elemento;
            }
        }
        return maximo;
    }

    // Wildcards
    public static void imprimirLista(List<?> lista) {
        for (Object elemento : lista) {
            System.out.print(elemento + " ");
        }
        System.out.println();
    }

    // Wildcard com upper bound
    public static double somaNumeros(List<? extends Number> numeros) {
        double soma = 0.0;
        for (Number num : numeros) {
            soma += num.doubleValue();
        }
        return soma;
    }

    // Wildcard com lower bound
    public static void adicionarNumeros(List<? super Integer> lista) {
        for (int i = 1; i <= 5; i++) {
            lista.add(i);
        }
    }

    public static void main(String[] args) {
        System.out.println("=== GENERICS FUNDAMENTOS ===");

        // Usando classe genérica
        Caixa<String> caixaString = new Caixa<>();
        caixaString.armazenar("Hello Generics!");
        System.out.println("Caixa String: " + caixaString.obter());

        Caixa<Integer> caixaInt = new Caixa<>();
        caixaInt.armazenar(42);
        System.out.println("Caixa Integer: " + caixaInt.obter());

        // Usando classe com múltiplos tipos
        Par<String, Integer> par = new Par<>("Idade", 25);
        System.out.println("Par: " + par);

        Par<Integer, String> parInvertido = new Par<>(1, "Um");
        System.out.println("Par Invertido: " + parInvertido);

        // Usando método genérico
        System.out.println("\n=== MÉTODOS GENÉRICOS ===");

        Integer[] numerosInt = {1, 2, 3, 4, 5};
        String[] palavras = {"Java", "Generics", "Coleções"};
        Double[] decimais = {1.1, 2.2, 3.3};

        System.out.print("Array de inteiros: ");
        imprimirArray(numerosInt);

        System.out.print("Array de strings: ");
        imprimirArray(palavras);

        System.out.print("Array de decimais: ");
        imprimirArray(decimais);

        // Método com tipo limitado
        System.out.println("\nMáximo de inteiros: " + encontrarMaximo(numerosInt));
        System.out.println("Máximo de decimais: " + encontrarMaximo(decimais));
        System.out.println("Máximo de strings: " + encontrarMaximo(palavras));

        // Wildcards
        System.out.println("\n=== WILDCARDS ===");

        List<Integer> listaInt = Arrays.asList(1, 2, 3);
        List<String> listaStr = Arrays.asList("A", "B", "C");
        List<Double> listaDouble = Arrays.asList(1.1, 2.2, 3.3);

        System.out.print("Lista de inteiros: ");
        imprimirLista(listaInt);

        System.out.print("Lista de strings: ");
        imprimirLista(listaStr);

        // Upper bound wildcard
        System.out.println("Soma de inteiros: " + somaNumeros(listaInt));
        System.out.println("Soma de decimais: " + somaNumeros(listaDouble));

        // Lower bound wildcard
        List<Number> listaNumeros = new ArrayList<>();
        adicionarNumeros(listaNumeros);
        System.out.println("Lista após adicionar números: " + listaNumeros);

        // Generics e herança
        System.out.println("\n=== GENERICS E HERANÇA ===");

        List<Integer> integers = new ArrayList<>();
        List<Number> numbers = new ArrayList<>();

        // integers = numbers; // ERRO de compilação!
        // numbers = integers; // ERRO de compilação!

        // Mas isso é permitido com wildcards
        List<? extends Number> numerosExtends = integers; // OK
        List<? super Integer> integersSuper = numbers; // OK

        System.out.println("Wildcard com extends: " + numerosExtends.getClass());
        System.out.println("Wildcard com super: " + integersSuper.getClass());
    }
}
```

### **8.2.7 Generics Avançados e Type Erasure**

**Exemplo 8.7: Generics Avançados**

```java
import java.lang.reflect.*;
import java.util.*;

public class ExemploGenericsAvancado {

    // Classe genérica com herança
    static class Container<T> {
        protected T item;

        public Container(T item) {
            this.item = item;
        }

        public T getItem() {
            return item;
        }

        public void setItem(T item) {
            this.item = item;
        }

        public void imprimirTipo() {
            System.out.println("Tipo do container: " + 
                    (item != null ? item.getClass().getSimpleName() : "null"));
        }
    }

    // Herança com tipo específico
    static class StringContainer extends Container<String> {
        public StringContainer(String item) {
            super(item);
        }

        // Método específico para strings
        public int comprimento() {
            return item != null ? item.length() : 0;
        }
    }

    // Herança com tipo genérico
    static class DuploContainer<T, U> extends Container<T> {
        private U segundoItem;

        public DuploContainer(T primeiroItem, U segundoItem) {
            super(primeiroItem);
            this.segundoItem = segundoItem;
        }

        public U getSegundoItem() {
            return segundoItem;
        }

        public void setSegundoItem(U segundoItem) {
            this.segundoItem = segundoItem;
        }

        @Override
        public void imprimirTipo() {
            System.out.println("Tipos: T=" + 
                    (item != null ? item.getClass().getSimpleName() : "null") +
                    ", U=" + (segundoItem != null ? segundoItem.getClass().getSimpleName() : "null"));
        }
    }

    // Interface genérica
    interface Repositorio<T, ID> {
        void salvar(T entidade);
        T buscarPorId(ID id);
        List<T> buscarTodos();
        void deletar(ID id);
    }

    // Implementação de interface genérica
    static class RepositorioMemoria<T, ID> implements Repositorio<T, ID> {
        private Map<ID, T> armazenamento = new HashMap<>();
        private ID proximoId;

        @SuppressWarnings("unchecked")
        public RepositorioMemoria() {
            // Simulação de geração de ID
            this.proximoId = (ID) Integer.valueOf(0);
        }

        @SuppressWarnings("unchecked")
        private ID gerarProximoId() {
            if (proximoId instanceof Integer) {
                Integer idInt = (Integer) proximoId;
                proximoId = (ID) Integer.valueOf(idInt + 1);
                return (ID) Integer.valueOf(idInt);
            }
            return proximoId;
        }

        @Override
        public void salvar(T entidade) {
            ID id = gerarProximoId();
            armazenamento.put(id, entidade);
            System.out.println("Salvo: " + entidade + " com ID: " + id);
        }

        @Override
        public T buscarPorId(ID id) {
            return armazenamento.get(id);
        }

        @Override
        public List<T> buscarTodos() {
            return new ArrayList<>(armazenamento.values());
        }

        @Override
        public void deletar(ID id) {
            armazenamento.remove(id);
            System.out.println("Deletado ID: " + id);
        }
    }

    // Demonstração de type erasure
    public static void demonstrarTypeErasure() {
        System.out.println("\n=== TYPE ERASURE ===");

        List<String> listaStrings = new ArrayList<>();
        List<Integer> listaIntegers = new ArrayList<>();

        // Em tempo de compilação, tipos são diferentes
        listaStrings.add("Texto");
        listaIntegers.add(42);

        // Em tempo de execução, o tipo genérico é apagado
        System.out.println("Tipo de listaStrings: " + listaStrings.getClass());
        System.out.println("Tipo de listaIntegers: " + listaIntegers.getClass());
        System.out.println("São do mesmo tipo? " + 
                (listaStrings.getClass() == listaIntegers.getClass()));

        // Reflexão para investigar type erasure
        try {
            Method metodoAdd = ArrayList.class.getMethod("add", Object.class);
            System.out.println("Método add encontrado: " + metodoAdd);
            
            // Podemos adicionar qualquer tipo devido ao type erasure
            @SuppressWarnings("unchecked")
            List<String> lista = (List<String>) listaStrings;
            Method m = lista.getClass().getMethod("add", Object.class);
            m.invoke(lista, 123); // Adicionando Integer em List<String>!
            
            System.out.println("Lista após adição via reflexão: " + lista);
        } catch (Exception e) {
            e.printStackTrace();
        }
    }

    // Bridge methods
    static class BridgeMethodExample<T> {
        public void setValue(T value) {
            System.out.println("BridgeMethodExample.setValue: " + value);
        }
    }

    static class StringBridgeExample extends BridgeMethodExample<String> {
        @Override
        public void setValue(String value) {
            System.out.println("StringBridgeExample.setValue: " + value);
        }
    }

    public static void main(String[] args) {
        System.out.println("=== GENERICS AVANÇADOS ===");

        // Uso das classes genéricas com herança
        Container<Integer> containerInt = new Container<>(42);
        containerInt.imprimirTipo();

        StringContainer stringContainer = new StringContainer("Hello");
        stringContainer.imprimirTipo();
        System.out.println("Comprimento: " + stringContainer.comprimento());

        DuploContainer<String, Integer> duploContainer = 
                new DuploContainer<>("Texto", 100);
        duploContainer.imprimirTipo();

        // Uso do repositório genérico
        System.out.println("\n=== REPOSITÓRIO GENÉRICO ===");

        Repositorio<String, Integer> repositorioStrings = new RepositorioMemoria<>();
        repositorioStrings.salvar("Primeiro item");
        repositorioStrings.salvar("Segundo item");

        System.out.println("Todos os itens: " + repositorioStrings.buscarTodos());
        System.out.println("Item com ID 0: " + repositorioStrings.buscarPorId(0));

        repositorioStrings.deletar(1);

        // Repositório com outro tipo
        Repositorio<Double, String> repositorioDoubles = new RepositorioMemoria<>();
        repositorioDoubles.salvar(3.14);
        repositorioDoubles.salvar(2.71);

        System.out.println("Doubles: " + repositorioDoubles.buscarTodos());

        // Demonstração de type erasure
        demonstrarTypeErasure();

        // Bridge methods
        System.out.println("\n=== BRIDGE METHODS ===");
        
        StringBridgeExample bridgeExample = new StringBridgeExample();
        bridgeExample.setValue("Teste Bridge");
        
        // Investigando métodos com reflexão
        Method[] methods = StringBridgeExample.class.getDeclaredMethods();
        for (Method method : methods) {
            System.out.println("Método: " + method + 
                    ", tipo retorno: " + method.getReturnType() +
                    ", bridge: " + method.isBridge());
        }
    }
}
```

## **8.3 Exercícios Práticos**

### **Exercício 8.1: Sistema de Gerenciamento de Biblioteca**

```java
import java.util.*;
import java.util.stream.Collectors;

public class SistemaBiblioteca {

    static class Livro implements Comparable<Livro> {
        private String isbn;
        private String titulo;
        private String autor;
        private int anoPublicacao;
        private boolean disponivel;

        public Livro(String isbn, String titulo, String autor, int anoPublicacao) {
            this.isbn = isbn;
            this.titulo = titulo;
            this.autor = autor;
            this.anoPublicacao = anoPublicacao;
            this.disponivel = true;
        }

        // Getters e Setters
        public String getIsbn() { return isbn; }
        public String getTitulo() { return titulo; }
        public String getAutor() { return autor; }
        public int getAnoPublicacao() { return anoPublicacao; }
        public boolean isDisponivel() { return disponivel; }
        public void setDisponivel(boolean disponivel) { this.disponivel = disponivel; }

        @Override
        public boolean equals(Object o) {
            if (this == o) return true;
            if (o == null || getClass() != o.getClass()) return false;
            Livro livro = (Livro) o;
            return Objects.equals(isbn, livro.isbn);
        }

        @Override
        public int hashCode() {
            return Objects.hash(isbn);
        }

        @Override
        public int compareTo(Livro outro) {
            return this.titulo.compareTo(outro.titulo);
        }

        @Override
        public String toString() {
            return String.format("Livro{isbn='%s', titulo='%s', autor='%s', ano=%d, disponivel=%s}",
                    isbn, titulo, autor, anoPublicacao, disponivel ? "sim" : "não");
        }
    }

    static class Usuario {
        private String id;
        private String nome;
        private String email;
        private Set<String> livrosEmprestados;

        public Usuario(String id, String nome, String email) {
            this.id = id;
            this.nome = nome;
            this.email = email;
            this.livrosEmprestados = new HashSet<>();
        }

        // Getters e Setters
        public String getId() { return id; }
        public String getNome() { return nome; }
        public String getEmail() { return email; }
        public Set<String> getLivrosEmprestados() { return livrosEmprestados; }

        public boolean podePegarEmprestado() {
            return livrosEmprestados.size() < 3;
        }

        public void adicionarLivro(String isbn) {
            livrosEmprestados.add(isbn);
        }

        public void removerLivro(String isbn) {
            livrosEmprestados.remove(isbn);
        }

        @Override
        public String toString() {
            return String.format("Usuario{id='%s', nome='%s', email='%s', livrosEmprestados=%d}",
                    id, nome, email, livrosEmprestados.size());
        }
    }

    public static class Biblioteca {
        private Map<String, Livro> livrosPorIsbn;
        private Map<String, Usuario> usuariosPorId;
        private Map<String, Set<String>> livrosPorAutor;

        public Biblioteca() {
            this.livrosPorIsbn = new HashMap<>();
            this.usuariosPorId = new HashMap<>();
            this.livrosPorAutor = new HashMap<>();
        }

        // Métodos para livros
        public void adicionarLivro(Livro livro) {
            livrosPorIsbn.put(livro.getIsbn(), livro);
            
            // Indexar por autor
            livrosPorAutor
                .computeIfAbsent(livro.getAutor(), k -> new HashSet<>())
                .add(livro.getIsbn());
        }

        public Optional<Livro> buscarLivroPorIsbn(String isbn) {
            return Optional.ofNullable(livrosPorIsbn.get(isbn));
        }

        public List<Livro> buscarLivrosPorAutor(String autor) {
            return livrosPorAutor.getOrDefault(autor, Collections.emptySet())
                    .stream()
                    .map(livrosPorIsbn::get)
                    .filter(Objects::nonNull)
                    .collect(Collectors.toList());
        }

        public List<Livro> buscarLivrosPorTitulo(String titulo) {
            return livrosPorIsbn.values().stream()
                    .filter(livro -> livro.getTitulo().toLowerCase().contains(titulo.toLowerCase()))
                    .collect(Collectors.toList());
        }

        public List<Livro> listarLivrosDisponiveis() {
            return livrosPorIsbn.values().stream()
                    .filter(Livro::isDisponivel)
                    .sorted()
                    .collect(Collectors.toList());
        }

        // Métodos para usuários
        public void cadastrarUsuario(Usuario usuario) {
            usuariosPorId.put(usuario.getId(), usuario);
        }

        public Optional<Usuario> buscarUsuarioPorId(String id) {
            return Optional.ofNullable(usuariosPorId.get(id));
        }

        // Métodos de empréstimo
        public boolean emprestarLivro(String usuarioId, String isbn) {
            Optional<Usuario> usuarioOpt = buscarUsuarioPorId(usuarioId);
            Optional<Livro> livroOpt = buscarLivroPorIsbn(isbn);

            if (usuarioOpt.isPresent() && livroOpt.isPresent()) {
                Usuario usuario = usuarioOpt.get();
                Livro livro = livroOpt.get();

                if (livro.isDisponivel() && usuario.podePegarEmprestado()) {
                    livro.setDisponivel(false);
                    usuario.adicionarLivro(isbn);
                    return true;
                }
            }
            return false;
        }

        public boolean devolverLivro(String usuarioId, String isbn) {
            Optional<Usuario> usuarioOpt = buscarUsuarioPorId(usuarioId);
            Optional<Livro> livroOpt = buscarLivroPorIsbn(isbn);

            if (usuarioOpt.isPresent() && livroOpt.isPresent()) {
                Usuario usuario = usuarioOpt.get();
                Livro livro = livroOpt.get();

                if (usuario.getLivrosEmprestados().contains(isbn)) {
                    livro.setDisponivel(true);
                    usuario.removerLivro(isbn);
                    return true;
                }
            }
            return false;
        }

        // Estatísticas
        public Map<String, Long> contarLivrosPorAutor() {
            return livrosPorIsbn.values().stream()
                    .collect(Collectors.groupingBy(
                        Livro::getAutor,
                        Collectors.counting()
                    ));
        }

        public Map<Integer, Long> contarLivrosPorAno() {
            return livrosPorIsbn.values().stream()
                    .collect(Collectors.groupingBy(
                        Livro::getAnoPublicacao,
                        Collectors.counting()
                    ));
        }

        public List<Usuario> listarUsuariosComMaisEmprestimos() {
            return usuariosPorId.values().stream()
                    .sorted(Comparator.comparingInt(u -> -u.getLivrosEmprestados().size()))
                    .collect(Collectors.toList());
        }
    }

    public static void main(String[] args) {
        Biblioteca biblioteca = new Biblioteca();

        // Adicionando livros
        biblioteca.adicionarLivro(new Livro("001", "Dom Casmurro", "Machado de Assis", 1899));
        biblioteca.adicionarLivro(new Livro("002", "O Cortiço", "Aluísio Azevedo", 1890));
        biblioteca.adicionarLivro(new Livro("003", "Memórias Póstumas", "Machado de Assis", 1881));
        biblioteca.adicionarLivro(new Livro("004", "O Alienista", "Machado de Assis", 1882));
        biblioteca.adicionarLivro(new Livro("005", "Iracema", "José de Alencar", 1865));

        // Cadastrando usuários
        biblioteca.cadastrarUsuario(new Usuario("U1", "João Silva", "joao@email.com"));
        biblioteca.cadastrarUsuario(new Usuario("U2", "Maria Santos", "maria@email.com"));

        // Realizando empréstimos
        System.out.println("=== EMPRÉSTIMOS ===");
        boolean sucesso1 = biblioteca.emprestarLivro("U1", "001");
        System.out.println("Empréstimo 001 para U1: " + (sucesso1 ? "Sucesso" : "Falha"));

        boolean sucesso2 = biblioteca.emprestarLivro("U1", "002");
        System.out.println("Empréstimo 002 para U1: " + (sucesso2 ? "Sucesso" : "Falha"));

        boolean sucesso3 = biblioteca.emprestarLivro("U1", "003");
        System.out.println("Empréstimo 003 para U1: " + (sucesso3 ? "Sucesso" : "Falha"));

        boolean sucesso4 = biblioteca.emprestarLivro("U1", "004"); // Deve falhar (limite 3)
        System.out.println("Empréstimo 004 para U1: " + (sucesso4 ? "Sucesso" : "Falha"));

        // Buscas
        System.out.println("\n=== BUSCAS ===");
        System.out.println("Livros de Machado de Assis:");
        biblioteca.buscarLivrosPorAutor("Machado de Assis").forEach(System.out::println);

        System.out.println("\nLivros disponíveis:");
        biblioteca.listarLivrosDisponiveis().forEach(System.out::println);

        // Estatísticas
        System.out.println("\n=== ESTATÍSTICAS ===");
        System.out.println("Livros por autor:");
        biblioteca.contarLivrosPorAutor().forEach((autor, count) -> 
            System.out.println(" - " + autor + ": " + count));

        System.out.println("\nUsuários com mais empréstimos:");
        biblioteca.listarUsuariosComMaisEmprestimos().forEach(System.out::println);

        // Devolução
        System.out.println("\n=== DEVOLUÇÃO ===");
        boolean devolucao = biblioteca.devolverLivro("U1", "001");
        System.out.println("Devolução 001: " + (devolucao ? "Sucesso" : "Falha"));

        System.out.println("Livros disponíveis após devolução:");
        biblioteca.listarLivrosDisponiveis().forEach(System.out::println);
    }
}
```

### **Exercício 8.2: Implementação de HashMap Customizado**

```java
import java.util.*;

public class HashMapCustom<K, V> {

    static class Entry<K, V> {
        final K key;
        V value;
        Entry<K, V> next;

        Entry(K key, V value) {
            this.key = key;
            this.value = value;
        }

        public K getKey() { return key; }
        public V getValue() { return value; }
        public V setValue(V value) { 
            V old = this.value;
            this.value = value;
            return old;
        }

        @Override
        public String toString() {
            return key + "=" + value;
        }
    }

    private static final int CAPACIDADE_INICIAL = 16;
    private static final float FATOR_CARGA = 0.75f;

    private Entry<K, V>[] tabela;
    private int tamanho;
    private int capacidade;

    @SuppressWarnings("unchecked")
    public HashMapCustom() {
        this.tabela = new Entry[CAPACIDADE_INICIAL];
        this.capacidade = CAPACIDADE_INICIAL;
        this.tamanho = 0;
    }

    private int hash(K key) {
        return key == null ? 0 : Math.abs(key.hashCode()) % capacidade;
    }

    public void put(K key, V value) {
        if (tamanho >= capacidade * FATOR_CARGA) {
            redimensionar();
        }

        int indice = hash(key);
        Entry<K, V> novoEntry = new Entry<>(key, value);

        if (tabela[indice] == null) {
            tabela[indice] = novoEntry;
        } else {
            Entry<K, V> atual = tabela[indice];
            Entry<K, V> anterior = null;

            while (atual != null) {
                if (Objects.equals(atual.key, key)) {
                    atual.setValue(value);
                    return;
                }
                anterior = atual;
                atual = atual.next;
            }

            if (anterior != null) {
                anterior.next = novoEntry;
            }
        }
        tamanho++;
    }

    public V get(K key) {
        int indice = hash(key);
        Entry<K, V> atual = tabela[indice];

        while (atual != null) {
            if (Objects.equals(atual.key, key)) {
                return atual.value;
            }
            atual = atual.next;
        }
        return null;
    }

    public boolean containsKey(K key) {
        return get(key) != null;
    }

    public V remove(K key) {
        int indice = hash(key);
        Entry<K, V> atual = tabela[indice];
        Entry<K, V> anterior = null;

        while (atual != null) {
            if (Objects.equals(atual.key, key)) {
                if (anterior == null) {
                    tabela[indice] = atual.next;
                } else {
                    anterior.next = atual.next;
                }
                tamanho--;
                return atual.value;
            }
            anterior = atual;
            atual = atual.next;
        }
        return null;
    }

    public int size() {
        return tamanho;
    }

    public boolean isEmpty() {
        return tamanho == 0;
    }

    public Set<K> keySet() {
        Set<K> keys = new HashSet<>();
        for (Entry<K, V> entry : tabela) {
            Entry<K, V> atual = entry;
            while (atual != null) {
                keys.add(atual.key);
                atual = atual.next;
            }
        }
        return keys;
    }

    public Collection<V> values() {
        List<V> values = new ArrayList<>();
        for (Entry<K, V> entry : tabela) {
            Entry<K, V> atual = entry;
            while (atual != null) {
                values.add(atual.value);
                atual = atual.next;
            }
        }
        return values;
    }

    public Set<Map.Entry<K, V>> entrySet() {
        Set<Map.Entry<K, V>> entries = new HashSet<>();
        for (Entry<K, V> entry : tabela) {
            Entry<K, V> atual = entry;
            while (atual != null) {
                entries.add(new AbstractMap.SimpleEntry<>(atual.key, atual.value));
                atual = atual.next;
            }
        }
        return entries;
    }

    @SuppressWarnings("unchecked")
    private void redimensionar() {
        capacidade *= 2;
        Entry<K, V>[] novaTabela = new Entry[capacidade];
        Entry<K, V>[] tabelaAntiga = tabela;
        tabela = novaTabela;
        tamanho = 0;

        for (Entry<K, V> entry : tabelaAntiga) {
            Entry<K, V> atual = entry;
            while (atual != null) {
                put(atual.key, atual.value);
                atual = atual.next;
            }
        }
    }

    @Override
    public String toString() {
        StringBuilder sb = new StringBuilder();
        sb.append("{");
        boolean primeiro = true;
        for (Map.Entry<K, V> entry : entrySet()) {
            if (!primeiro) {
                sb.append(", ");
            }
            sb.append(entry.getKey()).append("=").append(entry.getValue());
            primeiro = false;
        }
        sb.append("}");
        return sb.toString();
    }

    public static void main(String[] args) {
        HashMapCustom<String, Integer> mapa = new HashMapCustom<>();

        // Teste de inserção
        mapa.put("Um", 1);
        mapa.put("Dois", 2);
        mapa.put("Três", 3);
        mapa.put("Quatro", 4);
        mapa.put("Cinco", 5);

        System.out.println("Mapa após inserções: " + mapa);
        System.out.println("Tamanho: " + mapa.size());

        // Teste de busca
        System.out.println("\n=== BUSCAS ===");
        System.out.println("get('Um'): " + mapa.get("Um"));
        System.out.println("get('Seis'): " + mapa.get("Seis"));
        System.out.println("containsKey('Três'): " + mapa.containsKey("Três"));

        // Teste de remoção
        System.out.println("\n=== REMOÇÃO ===");
        System.out.println("remove('Dois'): " + mapa.remove("Dois"));
        System.out.println("Mapa após remoção: " + mapa);
        System.out.println("Tamanho: " + mapa.size());

        // Teste de colisões
        System.out.println("\n=== TESTE DE COLISÕES ===");
        HashMapCustom<Integer, String> mapaColisoes = new HashMapCustom<>();
        for (int i = 0; i < 20; i++) {
            mapaColisoes.put(i, "Valor " + i);
        }
        System.out.println("Mapa com colisões: " + mapaColisoes);
        System.out.println("Tamanho: " + mapaColisoes.size());
        System.out.println("Keys: " + mapaColisoes.keySet());
        System.out.println("Values: " + mapaColisoes.values());

        // Performance
        System.out.println("\n=== PERFORMANCE ===");
        long inicio = System.currentTimeMillis();
        HashMapCustom<Integer, Integer> grandeMapa = new HashMapCustom<>();
        for (int i = 0; i < 10000; i++) {
            grandeMapa.put(i, i * 2);
        }
        long fim = System.currentTimeMillis();
        System.out.println("Tempo para 10000 inserções: " + (fim - inicio) + "ms");
    }
}
```

## **8.4 Caso Prático: Sistema de Cache com Generics**

```java
import java.util.*;
import java.util.concurrent.*;

public class Cache<K, V> {

    private final Map<K, V> armazenamento;
    private final Queue<K> ordemAcesso;
    private final int capacidadeMaxima;
    private final long tempoExpiracaoMs;
    
    // Estatísticas
    private int hits;
    private int misses;

    public Cache(int capacidadeMaxima, long tempoExpiracaoMs) {
        this.capacidadeMaxima = capacidadeMaxima;
        this.tempoExpiracaoMs = tempoExpiracaoMs;
        this.armazenamento = new ConcurrentHashMap<>();
        this.ordemAcesso = new ConcurrentLinkedQueue<>();
        this.hits = 0;
        this.misses = 0;
    }

    public void put(K key, V value) {
        synchronized (armazenamento) {
            if (armazenamento.size() >= capacidadeMaxima) {
                removerMenosRecente();
            }
            
            armazenamento.put(key, value);
            atualizarOrdemAcesso(key);
            
            // Agendar expiração se necessário
            if (tempoExpiracaoMs > 0) {
                agendarExpiracao(key);
            }
        }
    }

    public Optional<V> get(K key) {
        V value = armazenamento.get(key);
        
        if (value != null) {
            hits++;
            atualizarOrdemAcesso(key);
            return Optional.of(value);
        } else {
            misses++;
            return Optional.empty();
        }
    }

    public boolean containsKey(K key) {
        return armazenamento.containsKey(key);
    }

    public V remove(K key) {
        synchronized (armazenamento) {
            ordemAcesso.remove(key);
            return armazenamento.remove(key);
        }
    }

    public void clear() {
        synchronized (armazenamento) {
            armazenamento.clear();
            ordemAcesso.clear();
            hits = 0;
            misses = 0;
        }
    }

    public int size() {
        return armazenamento.size();
    }

    public boolean isEmpty() {
        return armazenamento.isEmpty();
    }

    public Set<K> keySet() {
        return Collections.unmodifiableSet(armazenamento.keySet());
    }

    public Collection<V> values() {
        return Collections.unmodifiableCollection(armazenamento.values());
    }

    public double getTaxaAcerto() {
        int total = hits + misses;
        return total > 0 ? (double) hits / total : 0.0;
    }

    public Estatisticas getEstatisticas() {
        return new Estatisticas(hits, misses, armazenamento.size());
    }

    private void atualizarOrdemAcesso(K key) {
        ordemAcesso.remove(key); // Remove se já existir
        ordemAcesso.offer(key);  // Adiciona no final
    }

    private void removerMenosRecente() {
        K menosRecente = ordemAcesso.poll();
        if (menosRecente != null) {
            armazenamento.remove(menosRecente);
        }
    }

    private void agendarExpiracao(K key) {
        if (tempoExpiracaoMs > 0) {
            Timer timer = new Timer(true);
            timer.schedule(new TimerTask() {
                @Override
                public void run() {
                    remove(key);
                }
            }, tempoExpiracaoMs);
        }
    }

    public static class Estatisticas {
        private final int hits;
        private final int misses;
        private final int tamanho;

        public Estatisticas(int hits, int misses, int tamanho) {
            this.hits = hits;
            this.misses = misses;
            this.tamanho = tamanho;
        }

        public int getHits() { return hits; }
        public int getMisses() { return misses; }
        public int getTamanho() { return tamanho; }
        public double getTaxaAcerto() {
            int total = hits + misses;
            return total > 0 ? (double) hits / total : 0.0;
        }

        @Override
        public String toString() {
            return String.format(
                "Estatisticas{hits=%d, misses=%d, tamanho=%d, taxaAcerto=%.2f}",
                hits, misses, tamanho, getTaxaAcerto()
            );
        }
    }

    public static void main(String[] args) throws InterruptedException {
        System.out.println("=== SISTEMA DE CACHE ===");

        // Cache com capacidade 3 e expiração de 2 segundos
        Cache<String, String> cache = new Cache<>(3, 2000);

        // Teste de capacidade
        cache.put("A", "Alice");
        cache.put("B", "Bob");
        cache.put("C", "Charlie");
        cache.put("D", "Diana"); // Deve remover "A" (menos recente)

        System.out.println("Cache após inserções: " + cache.keySet());
        
        // Teste de acesso para atualizar ordem
        cache.get("B"); // Acesso a "B" torna-o mais recente
        cache.put("E", "Eva"); // Deve remover "C" (menos recente)

        System.out.println("Cache após acesso e nova inserção: " + cache.keySet());

        // Teste de estatísticas
        cache.get("B"); // hit
        cache.get("X"); // miss
        cache.get("E"); // hit

        System.out.println("Estatísticas: " + cache.getEstatisticas());
        System.out.println("Taxa de acerto: " + cache.getTaxaAcerto());

        // Teste de expiração
        cache.put("Temporario", "Valor temporário");
        System.out.println("Antes da expiração: " + cache.containsKey("Temporario"));
        
        Thread.sleep(2500); // Aguarda expiração
        System.out.println("Após expiração: " + cache.containsKey("Temporario"));

        // Cache com diferentes tipos
        Cache<Integer, List<String>> cacheComplexo = new Cache<>(5, 0);
        cacheComplexo.put(1, Arrays.asList("Java", "Python"));
        cacheComplexo.put(2, Arrays.asList("C++", "JavaScript"));

        System.out.println("\nCache complexo: " + cacheComplexo.keySet());
        cacheComplexo.get(1).ifPresent(lista -> 
            System.out.println("Valor da chave 1: " + lista)
        );
    }
}
```

## **8.5 Questionário de Revisão**

**Questão 1:** Qual a diferença entre ArrayList e LinkedList?
- A) ArrayList tem acesso rápido por índice, LinkedList tem inserções rápidas
- B) LinkedList é sempre mais rápido que ArrayList
- C) ArrayList é thread-safe, LinkedList não é

**Questão 2:** O que é type erasure em Generics?
- A) Remoção de informações de tipo em tempo de compilação
- B) Remoção de informações de tipo em tempo de execução
- C) Erro ao usar tipos genéricos

**Questão 3:** Qual interface implementa uma coleção que não permite duplicatas?
- A) List
- B) Set
- C) Queue

**Questão 4:** Para que serve o wildcard `<? extends Number>`?
- A) Aceita Number e seus subtipos
- B) Aceita Number e seus supertipos
- C) Aceita qualquer tipo

**Questão 5:** Qual a vantagem do HashMap sobre o TreeMap?
- A) Performance O(1) vs O(log n) para operações básicas
- B) Mantém ordem de inserção
- C) É thread-safe

## **8.6 Laboratório Prático**

**Projeto: Sistema de Agenda de Contatos**

```java
// Implemente um sistema de agenda de contatos que:
// 1. Armazene contatos com nome, telefones múltiplos e emails
// 2. Permita buscar por nome, telefone ou email
// 3. Suporte grupos de contatos
// 4. Gerencie favoritos
// 5. Exporte/importe contatos

// Use: Map, Set, List, Generics, Collections API
```

## **8.7 Material de Apoio**

**Resumo das Principais Interfaces:**

**Collection:**
- `add()`, `remove()`, `contains()`, `size()`, `isEmpty()`
- `iterator()`, `toArray()`, `stream()`

**List:**
- `get(index)`, `set(index, element)`, `add(index, element)`
- `indexOf()`, `lastIndexOf()`, `subList()`

**Set:**
- Herda de Collection, garante unicidade
- `HashSet`: não ordenado, O(1)
- `TreeSet`: ordenado, O(log n)
- `LinkedHashSet`: ordem de inserção, O(1)

**Map:**
- `put(key, value)`, `get(key)`, `remove(key)`
- `keySet()`, `values()`, `entrySet()`
- `HashMap`, `TreeMap`, `LinkedHashMap`

**Queue:**
- `offer()`, `poll()`, `peek()`
- `LinkedList`, `PriorityQueue`, `ArrayDeque`

**Generics Best Practices:**
- Use tipos genéricos para type safety
- Prefira `List<String>` sobre `List` (raw types)
- Use wildcards para flexibilidade: `<?>`, `<? extends T>`, `<? super T>`
- Evite usar generics com arrays: `List<String>[]` é perigoso

**Dicas de Performance:**
- Use `ArrayList` para acesso por índice frequente
- Use `LinkedList` para muitas inserções/remoções no meio
- Use `HashSet`/`HashMap` para operações O(1)
- Use `Collections.synchronizedXXX()` para thread-safety
- Considere `ConcurrentHashMap` para acesso concorrente

---

**Próximo Módulo: Streams API e Lambda Expressions**

Preparado para explorar a programação funcional em Java e a poderosa Streams API?

---

# **Módulo 9: Streams API e Lambda Expressions**

## **9.1 Objetivos do Módulo**

- Compreender expressões lambda e funções anônimas
- Dominar a Streams API para processamento de coleções
- Aprender a usar method references
- Conhecer as principais operações intermediárias e terminais
- Aplicar programação funcional em Java
- Trabalhar com Optional e evitar NullPointerException

## **9.2 Conteúdo Programático**

### **9.2.1 Lambda Expressions**

**Exemplo 9.1: Introdução a Lambda Expressions**

```java
import java.util.*;
import java.util.function.*;

public class ExemploLambda {

    public static void main(String[] args) {
        System.out.println("=== LAMBDA EXPRESSIONS ===");

        // Antes do Java 8: classes anônimas
        Comparator<String> comparadorAnonimo = new Comparator<String>() {
            @Override
            public int compare(String s1, String s2) {
                return s1.compareTo(s2);
            }
        };

        // Com Lambda (equivalente)
        Comparator<String> comparadorLambda = (s1, s2) -> s1.compareTo(s2);

        // Exemplos de sintaxe lambda
        Function<String, Integer> stringParaInt = s -> Integer.parseInt(s);
        Function<String, Integer> stringParaInt2 = Integer::parseInt; // Method reference

        Consumer<String> impressora = s -> System.out.println(s);
        Consumer<String> impressora2 = System.out::println;

        Supplier<Date> fornecedorData = () -> new Date();
        Supplier<Date> fornecedorData2 = Date::new;

        Predicate<String> predicadoVazio = s -> s.isEmpty();
        Predicate<String> predicadoVazio2 = String::isEmpty;

        // Uso prático
        List<String> palavras = Arrays.asList("Java", "Python", "C", "JavaScript", "Ruby");

        // Ordenação com lambda
        Collections.sort(palavras, (s1, s2) -> s1.length() - s2.length());
        System.out.println("Ordenado por length: " + palavras);

        // Ou usando Comparator.comparing
        Collections.sort(palavras, Comparator.comparing(String::length));
        System.out.println("Ordenado por length (method reference): " + palavras);

        // Reverse
        Collections.sort(palavras, Comparator.comparing(String::length).reversed());
        System.out.println("Ordenado por length reverso: " + palavras);

        // Múltiplos critérios
        Collections.sort(palavras, Comparator.comparing(String::length)
                                            .thenComparing(Comparator.naturalOrder()));
        System.out.println("Ordenado por length e depois natural: " + palavras);

        // Demonstração de interfaces funcionais
        demonstrarInterfacesFuncionais();
    }

    public static void demonstrarInterfacesFuncionais() {
        System.out.println("\n=== INTERFACES FUNCIONAIS ===");

        // Predicate (testa uma condição)
        Predicate<Integer> ehPar = n -> n % 2 == 0;
        System.out.println("4 é par? " + ehPar.test(4));
        System.out.println("5 é par? " + ehPar.test(5));

        // Function (transforma um valor)
        Function<String, Integer> tamanhoString = String::length;
        System.out.println("Tamanho de 'Java': " + tamanhoString.apply("Java"));

        // Consumer (consome um valor)
        Consumer<String> saudacao = nome -> System.out.println("Olá, " + nome + "!");
        saudacao.accept("Maria");

        // Supplier (fornece um valor)
        Supplier<Double> numeroAleatorio = () -> Math.random();
        System.out.println("Número aleatório: " + numeroAleatorio.get());

        // UnaryOperator (Function onde entrada e saída são do mesmo tipo)
        UnaryOperator<String> maiusculas = String::toUpperCase;
        System.out.println("java em maiúsculas: " + maiusculas.apply("java"));

        // BinaryOperator (dois parâmetros do mesmo tipo, retorno do mesmo tipo)
        BinaryOperator<Integer> soma = Integer::sum;
        System.out.println("Soma de 10 + 20: " + soma.apply(10, 20));

        // BiFunction (dois parâmetros, retorno de outro tipo)
        BiFunction<String, String, String> concatenador = (s1, s2) -> s1 + " " + s2;
        System.out.println("Concatenado: " + concatenador.apply("Java", "8"));

        // BiPredicate (dois parâmetros, retorno boolean)
        BiPredicate<String, String> comecaCom = (s1, s2) -> s1.startsWith(s2);
        System.out.println("'Java' começa com 'Ja'? " + comecaCom.test("Java", "Ja"));

        // Composição de funções
        Function<Integer, Integer> dobro = n -> n * 2;
        Function<Integer, Integer> incremento = n -> n + 1;

        Function<Integer, Integer> dobroMaisIncremento = dobro.andThen(incremento);
        Function<Integer, Integer> incrementoMaisDobro = dobro.compose(incremento);

        System.out.println("Dobro e depois incremento de 5: " + dobroMaisIncremento.apply(5));
        System.out.println("Incremento e depois dobro de 5: " + incrementoMaisDobro.apply(5));

        // Combinando predicates
        Predicate<Integer> ehMaiorQue10 = n -> n > 10;
        Predicate<Integer> ehMenorQue20 = n -> n < 20;

        Predicate<Integer> entre10e20 = ehMaiorQue10.and(ehMenorQue20);
        System.out.println("15 está entre 10 e 20? " + entre10e20.test(15));

        Predicate<String> naoEhVazio = Predicate.not(String::isEmpty);
        System.out.println("'' não é vazio? " + naoEhVazio.test(""));
    }
}
```

### **9.2.2 Method References**

**Exemplo 9.2: Method References**

```java
import java.util.*;
import java.util.function.*;

public class ExemploMethodReference {

    static class Pessoa {
        private String nome;
        private int idade;

        public Pessoa(String nome, int idade) {
            this.nome = nome;
            this.idade = idade;
        }

        public String getNome() { return nome; }
        public int getIdade() { return idade; }

        public static int compararPorIdade(Pessoa p1, Pessoa p2) {
            return Integer.compare(p1.idade, p2.idade);
        }

        public static boolean ehMaiorDeIdade(Pessoa p) {
            return p.idade >= 18;
        }

        @Override
        public String toString() {
            return String.format("Pessoa{nome='%s', idade=%d}", nome, idade);
        }
    }

    public static void main(String[] args) {
        System.out.println("=== METHOD REFERENCES ===");

        List<Pessoa> pessoas = Arrays.asList(
            new Pessoa("Alice", 25),
            new Pessoa("Bob", 17),
            new Pessoa("Charlie", 30),
            new Pessoa("Diana", 16)
        );

        // Referência a método estático
        Function<String, Integer> conversor = Integer::parseInt;
        System.out.println("String '123' para int: " + conversor.apply("123"));

        // Referência a método de instância de um objeto específico
        String prefixo = "Mr. ";
        Function<String, String> adicionarPrefixoSr = prefixo::concat;
        System.out.println(adicionarPrefixoSr.apply("Smith"));

        // Referência a método de instância de um tipo arbitrário
        Function<String, String> paraMaiusculas = String::toUpperCase;
        System.out.println("java em maiúsculas: " + paraMaiusculas.apply("java"));

        // Referência a construtor
        Supplier<List<String>> supplierLista = ArrayList::new;
        List<String> novaLista = supplierLista.get();
        novaLista.add("Elemento");
        System.out.println("Nova lista: " + novaLista);

        // Aplicações práticas
        System.out.println("\n=== APLICAÇÕES PRÁTICAS ===");

        // Ordenação com method reference
        System.out.println("Pessoas ordenadas por nome:");
        pessoas.sort(Comparator.comparing(Pessoa::getNome));
        pessoas.forEach(System.out::println);

        System.out.println("\nPessoas ordenadas por idade:");
        pessoas.sort(Pessoa::compararPorIdade);
        pessoas.forEach(System.out::println);

        // Filtro com method reference
        System.out.println("\nMaiores de idade:");
        pessoas.stream()
              .filter(Pessoa::ehMaiorDeIdade)
              .forEach(System.out::println);

        // Mapping com method reference
        System.out.println("\nApenas nomes:");
        pessoas.stream()
              .map(Pessoa::getNome)
              .forEach(System.out::println);

        // System.out::println
        System.out.println("\nNúmeros de 1 a 5:");
        Arrays.asList(1, 2, 3, 4, 5).forEach(System.out::println);

        // Demonstração de todos os tipos
        demonstrarTiposMethodReference();
    }

    public static void demonstrarTiposMethodReference() {
        System.out.println("\n=== TIPOS DE METHOD REFERENCE ===");

        // 1. Referência a método estático
        Function<Double, Double> raizQuadrada = Math::sqrt;
        System.out.println("Raiz quadrada de 16: " + raizQuadrada.apply(16.0));

        // 2. Referência a método de instância de objeto particular
        String str = "Java Programming";
        Supplier<String> toLowerCase = str::toLowerCase;
        System.out.println("String em minúsculas: " + toLowerCase.get());

        // 3. Referência a método de instância de tipo arbitrário
        Function<String, Integer> indexOfSpace = String::indexOf;
        System.out.println("Índice do espaço em 'Java Programming': " + 
                          indexOfSpace.apply("Java Programming"));

        // 4. Referência a construtor
        Supplier<HashMap<String, Integer>> mapSupplier = HashMap::new;
        Map<String, Integer> novoMapa = mapSupplier.get();
        novoMapa.put("Chave", 42);
        System.out.println("Novo mapa: " + novoMapa);

        // Referência a construtor com parâmetros
        Function<String, Pessoa> criadorPessoa = Pessoa::new;
        Pessoa novaPessoa = criadorPessoa.apply("Eva");
        System.out.println("Nova pessoa: " + novaPessoa);
    }
}
```

### **9.2.3 Streams API - Fundamentos**

**Exemplo 9.3: Introdução à Streams API**

```java
import java.util.*;
import java.util.stream.*;

public class ExemploStreams {

    public static void main(String[] args) {
        System.out.println("=== STREAMS API - FUNDAMENTOS ===");

        // Características das Streams
        System.out.println("• Não armazenam dados, apenas processam");
        System.out.println("• Não modificam a fonte original");
        System.out.println("• Operações lazy (adiem processamento)");
        System.out.println("• Podem ser sequenciais ou paralelas");

        // Criando Streams
        List<String> palavras = Arrays.asList("Java", "Python", "JavaScript", "C", "Ruby", "Go");

        System.out.println("\n=== CRIANDO STREAMS ===");

        // De coleção
        Stream<String> stream1 = palavras.stream();

        // De array
        String[] array = {"A", "B", "C"};
        Stream<String> stream2 = Arrays.stream(array);

        // De valores
        Stream<String> stream3 = Stream.of("X", "Y", "Z");

        // Sequência numérica
        IntStream stream4 = IntStream.range(1, 6); // 1, 2, 3, 4, 5
        IntStream stream5 = IntStream.rangeClosed(1, 5); // 1, 2, 3, 4, 5

        // Stream infinita
        Stream<Integer> stream6 = Stream.iterate(0, n -> n + 2); // 0, 2, 4, 6...
        Stream<Double> stream7 = Stream.generate(Math::random); // números aleatórios

        // Operações básicas
        System.out.println("\n=== OPERAÇÕES BÁSICAS ===");

        System.out.println("Lista original: " + palavras);

        // Filter
        System.out.println("\nFilter - Linguagens com mais de 3 caracteres:");
        palavras.stream()
               .filter(s -> s.length() > 3)
               .forEach(System.out::println);

        // Map
        System.out.println("\nMap - Transformando em maiúsculas:");
        palavras.stream()
               .map(String::toUpperCase)
               .forEach(System.out::println);

        // Map com transformação
        System.out.println("\nMap - Tamanho das palavras:");
        palavras.stream()
               .map(String::length)
               .forEach(tamanho -> System.out.print(tamanho + " "));

        // Sorted
        System.out.println("\n\nSorted - Ordem natural:");
        palavras.stream()
               .sorted()
               .forEach(p -> System.out.print(p + " "));

        System.out.println("\nSorted - Por tamanho:");
        palavras.stream()
               .sorted(Comparator.comparing(String::length))
               .forEach(p -> System.out.print(p + " "));

        // Distinct
        List<String> comDuplicatas = Arrays.asList("Java", "Python", "Java", "C", "Python");
        System.out.println("\n\nDistinct - Removendo duplicatas:");
        comDuplicatas.stream()
                    .distinct()
                    .forEach(p -> System.out.print(p + " "));

        // Limit e Skip
        System.out.println("\n\nLimit e Skip - Paginação:");
        palavras.stream()
               .skip(2)        // Pula os 2 primeiros
               .limit(3)       // Pega os próximos 3
               .forEach(p -> System.out.print(p + " "));

        // Operações terminais básicas
        System.out.println("\n\n=== OPERAÇÕES TERMINAIS ===");

        // forEach
        System.out.println("forEach:");
        palavras.forEach(p -> System.out.print(p + " "));

        // count
        long count = palavras.stream().count();
        System.out.println("\nCount: " + count);

        // collect
        List<String> filtradas = palavras.stream()
                                       .filter(s -> s.length() > 3)
                                       .collect(Collectors.toList());
        System.out.println("Collect to List: " + filtradas);

        // anyMatch, allMatch, noneMatch
        boolean temJava = palavras.stream().anyMatch(s -> s.equals("Java"));
        boolean todosTemJ = palavras.stream().allMatch(s -> s.contains("J"));
        boolean nenhumTemZ = palavras.stream().noneMatch(s -> s.contains("Z"));

        System.out.println("Tem Java? " + temJava);
        System.out.println("Todos tem 'J'? " + todosTemJ);
        System.out.println("Nenhum tem 'Z'? " + nenhumTemZ);

        // findFirst, findAny
        Optional<String> primeira = palavras.stream().findFirst();
        Optional<String> qualquer = palavras.stream().findAny();

        System.out.println("Primeira: " + primeira.orElse("Nenhuma"));
        System.out.println("Qualquer: " + qualquer.orElse("Nenhuma"));

        // Demonstração de lazy evaluation
        System.out.println("\n=== LAZY EVALUATION ===");
        Stream<String> streamLazy = palavras.stream()
                                          .filter(s -> {
                                              System.out.println("Filtrando: " + s);
                                              return s.length() > 3;
                                          })
                                          .map(s -> {
                                              System.out.println("Mapeando: " + s);
                                              return s.toUpperCase();
                                          });

        System.out.println("Stream criada, mas nenhuma operação executada ainda...");

        // A operação terminal força o processamento
        System.out.println("Chamando operação terminal:");
        streamLazy.forEach(System.out::println);
    }
}
```

### **9.2.4 Streams API - Operações Intermediárias**

**Exemplo 9.4: Operações Intermediárias Avançadas**

```java
import java.util.*;
import java.util.stream.*;

public class ExemploOperacoesIntermediarias {

    static class Produto {
        private String nome;
        private String categoria;
        private double preco;
        private int quantidade;

        public Produto(String nome, String categoria, double preco, int quantidade) {
            this.nome = nome;
            this.categoria = categoria;
            this.preco = preco;
            this.quantidade = quantidade;
        }

        // Getters
        public String getNome() { return nome; }
        public String getCategoria() { return categoria; }
        public double getPreco() { return preco; }
        public int getQuantidade() { return quantidade; }

        @Override
        public String toString() {
            return String.format("Produto{nome='%s', categoria='%s', preco=%.2f, quantidade=%d}",
                    nome, categoria, preco, quantidade);
        }
    }

    public static void main(String[] args) {
        System.out.println("=== OPERAÇÕES INTERMEDIÁRIAS AVANÇADAS ===");

        List<Produto> produtos = Arrays.asList(
            new Produto("Notebook", "Eletrônicos", 2500.00, 10),
            new Produto("Mouse", "Eletrônicos", 50.00, 50),
            new Produto("Teclado", "Eletrônicos", 150.00, 30),
            new Produto("Monitor", "Eletrônicos", 800.00, 15),
            new Produto("Cadeira", "Móveis", 500.00, 20),
            new Produto("Mesa", "Móveis", 300.00, 25),
            new Produto("Livro Java", "Livros", 80.00, 100),
            new Produto("Livro Python", "Livros", 70.00, 80),
            new Produto("Headphone", "Eletrônicos", 200.00, 40)
        );

        // Map vs FlatMap
        System.out.println("\n=== MAP vs FLATMAP ===");

        // Map: transformação 1-para-1
        System.out.println("Map - Apenas nomes:");
        produtos.stream()
               .map(Produto::getNome)
               .forEach(nome -> System.out.print(nome + " "));

        // FlatMap: transformação 1-para-muitos
        System.out.println("\n\nFlatMap - Quebrando strings em caracteres:");
        List<String> palavras = Arrays.asList("Java", "Stream");
        palavras.stream()
               .flatMap(palavra -> Arrays.stream(palavra.split("")))
               .forEach(caractere -> System.out.print(caractere + " "));

        // Exemplo prático de FlatMap
        System.out.println("\n\nFlatMap - Todos os produtos por categoria:");
        Map<String, List<Produto>> produtosPorCategoria = produtos.stream()
                .collect(Collectors.groupingBy(Produto::getCategoria));

        produtosPorCategoria.values().stream()
                          .flatMap(List::stream)
                          .forEach(System.out::println);

        // Operações de agrupamento e ordenação
        System.out.println("\n=== AGRUPAMENTO E ORDENAÇÃO ===");

        System.out.println("Ordenado por preço (crescente):");
        produtos.stream()
               .sorted(Comparator.comparing(Produto::getPreco))
               .forEach(p -> System.out.printf("%s: R$%.2f\n", p.getNome(), p.getPreco()));

        System.out.println("\nOrdenado por preço (decrescente):");
        produtos.stream()
               .sorted(Comparator.comparing(Produto::getPreco).reversed())
               .forEach(p -> System.out.printf("%s: R$%.2f\n", p.getNome(), p.getPreco()));

        System.out.println("\nOrdenado por categoria e depois preço:");
        produtos.stream()
               .sorted(Comparator.comparing(Produto::getCategoria)
                                .thenComparing(Produto::getPreco))
               .forEach(p -> System.out.printf("%s - %s: R$%.2f\n", 
                       p.getCategoria(), p.getNome(), p.getPreco()));

        // Peek - para debug
        System.out.println("\n=== PEEK (DEBUG) ===");
        List<String> nomesProcessados = produtos.stream()
               .filter(p -> p.getPreco() > 100.00)
               .peek(p -> System.out.println("Após filter > 100: " + p.getNome()))
               .map(Produto::getNome)
               .peek(nome -> System.out.println("Após map para nome: " + nome))
               .collect(Collectors.toList());

        System.out.println("Nomes processados: " + nomesProcessados);

        // Operações com tipos primitivos
        System.out.println("\n=== STREAMS DE TIPOS PRIMITIVOS ===");

        // IntStream, DoubleStream, LongStream
        System.out.println("Preços como DoubleStream:");
        DoubleStream precos = produtos.stream()
                                    .mapToDouble(Produto::getPreco);

        System.out.println("Soma: R$" + precos.sum());

        // Estatísticas
        DoubleSummaryStatistics stats = produtos.stream()
                                               .mapToDouble(Produto::getPreco)
                                               .summaryStatistics();

        System.out.println("\nEstatísticas de preços:");
        System.out.printf("Count: %d\n", stats.getCount());
        System.out.printf("Soma: R$%.2f\n", stats.getSum());
        System.out.printf("Mínimo: R$%.2f\n", stats.getMin());
        System.out.printf("Máximo: R$%.2f\n", stats.getMax());
        System.out.printf("Média: R$%.2f\n", stats.getAverage());

        // Operações de redução
        System.out.println("\n=== REDUCE ===");

        // Soma dos preços com reduce
        Optional<Double> somaPrecos = produtos.stream()
                                             .map(Produto::getPreco)
                                             .reduce(Double::sum);

        System.out.println("Soma dos preços: R$" + somaPrecos.orElse(0.0));

        // Soma com valor identidade
        double somaComIdentidade = produtos.stream()
                                          .map(Produto::getPreco)
                                          .reduce(0.0, Double::sum);

        System.out.println("Soma com identidade: R$" + somaComIdentidade);

        // Concatenação de nomes
        String nomesConcatenados = produtos.stream()
                                          .map(Produto::getNome)
                                          .reduce("", (s1, s2) -> s1 + ", " + s2);

        System.out.println("Nomes concatenados: " + nomesConcatenados);

        // Produto mais caro com reduce
        Optional<Produto> maisCaro = produtos.stream()
                                            .reduce((p1, p2) -> 
                                                p1.getPreco() > p2.getPreco() ? p1 : p2);

        maisCaro.ifPresent(p -> 
            System.out.println("Produto mais caro: " + p.getNome() + " - R$" + p.getPreco()));
    }
}
```

### **9.2.5 Streams API - Operações Terminais**

**Exemplo 9.5: Operações Terminais e Collectors**

```java
import java.util.*;
import java.util.stream.*;

public class ExemploOperacoesTerminais {

    static class Pessoa {
        private String nome;
        private int idade;
        private String cidade;

        public Pessoa(String nome, int idade, String cidade) {
            this.nome = nome;
            this.idade = idade;
            this.cidade = cidade;
        }

        // Getters
        public String getNome() { return nome; }
        public int getIdade() { return idade; }
        public String getCidade() { return cidade; }

        @Override
        public String toString() {
            return String.format("Pessoa{nome='%s', idade=%d, cidade='%s'}", nome, idade, cidade);
        }
    }

    public static void main(String[] args) {
        System.out.println("=== OPERAÇÕES TERMINAIS E COLLECTORS ===");

        List<Pessoa> pessoas = Arrays.asList(
            new Pessoa("Alice", 25, "São Paulo"),
            new Pessoa("Bob", 30, "Rio de Janeiro"),
            new Pessoa("Charlie", 22, "São Paulo"),
            new Pessoa("Diana", 28, "Belo Horizonte"),
            new Pessoa("Eva", 35, "Rio de Janeiro"),
            new Pessoa("Frank", 19, "São Paulo"),
            new Pessoa("Grace", 32, "Curitiba")
        );

        // Collectors.toList()
        System.out.println("\n=== COLETANDO RESULTADOS ===");

        List<String> nomes = pessoas.stream()
                                   .map(Pessoa::getNome)
                                   .collect(Collectors.toList());
        System.out.println("Nomes: " + nomes);

        // Collectors.toSet()
        Set<String> cidades = pessoas.stream()
                                    .map(Pessoa::getCidade)
                                    .collect(Collectors.toSet());
        System.out.println("Cidades únicas: " + cidades);

        // Collectors.toMap()
        Map<String, Integer> nomeParaIdade = pessoas.stream()
                .collect(Collectors.toMap(
                    Pessoa::getNome,
                    Pessoa::getIdade
                ));
        System.out.println("Mapa nome->idade: " + nomeParaIdade);

        // Collectors.joining()
        String todosNomes = pessoas.stream()
                                  .map(Pessoa::getNome)
                                  .collect(Collectors.joining(", "));
        System.out.println("Nomes concatenados: " + todosNomes);

        // Agrupamento
        System.out.println("\n=== AGRUPAMENTO ===");

        Map<String, List<Pessoa>> porCidade = pessoas.stream()
                .collect(Collectors.groupingBy(Pessoa::getCidade));

        System.out.println("Pessoas por cidade:");
        porCidade.forEach((cidade, lista) -> {
            System.out.println(cidade + ": " + lista.stream()
                                                   .map(Pessoa::getNome)
                                                   .collect(Collectors.joining(", ")));
        });

        // Agrupamento com contagem
        Map<String, Long> contagemPorCidade = pessoas.stream()
                .collect(Collectors.groupingBy(
                    Pessoa::getCidade,
                    Collectors.counting()
                ));
        System.out.println("Contagem por cidade: " + contagemPorCidade);

        // Agrupamento com mapeamento
        Map<String, Set<String>> nomesPorCidade = pessoas.stream()
                .collect(Collectors.groupingBy(
                    Pessoa::getCidade,
                    Collectors.mapping(Pessoa::getNome, Collectors.toSet())
                ));
        System.out.println("Nomes por cidade: " + nomesPorCidade);

        // Partitioning (divisão binária)
        System.out.println("\n=== PARTITIONING ===");

        Map<Boolean, List<Pessoa>> maioridade = pessoas.stream()
                .collect(Collectors.partitioningBy(p -> p.getIdade() >= 18));

        System.out.println("Maiores de idade: " + 
            maioridade.get(true).stream()
                     .map(Pessoa::getNome)
                     .collect(Collectors.joining(", ")));

        System.out.println("Menores de idade: " + 
            maioridade.get(false).stream()
                     .map(Pessoa::getNome)
                     .collect(Collectors.joining(", ")));

        // Estatísticas com agrupamento
        System.out.println("\n=== ESTATÍSTICAS ===");

        Map<String, Double> idadeMediaPorCidade = pessoas.stream()
                .collect(Collectors.groupingBy(
                    Pessoa::getCidade,
                    Collectors.averagingInt(Pessoa::getIdade)
                ));
        System.out.println("Idade média por cidade: " + idadeMediaPorCidade);

        Map<String, IntSummaryStatistics> statsPorCidade = pessoas.stream()
                .collect(Collectors.groupingBy(
                    Pessoa::getCidade,
                    Collectors.summarizingInt(Pessoa::getIdade)
                ));

        statsPorCidade.forEach((cidade, stat) -> {
            System.out.printf("%s: count=%d, avg=%.1f, min=%d, max=%d\n",
                    cidade, stat.getCount(), stat.getAverage(), stat.getMin(), stat.getMax());
        });

        // Colectors.collectingAndThen
        System.out.println("\n=== COLLECTING AND THEN ===");

        List<String> nomesImutaveis = pessoas.stream()
                .map(Pessoa::getNome)
                .collect(Collectors.collectingAndThen(
                    Collectors.toList(),
                    Collections::unmodifiableList
                ));
        System.out.println("Lista imutável: " + nomesImutaveis);

        // Operações de redução com Collectors
        System.out.println("\n=== REDUÇÃO COM COLLECTORS ===");

        Optional<Pessoa> maisVelho = pessoas.stream()
                .collect(Collectors.maxBy(Comparator.comparing(Pessoa::getIdade)));

        Optional<Pessoa> maisNovo = pessoas.stream()
                .collect(Collectors.minBy(Comparator.comparing(Pessoa::getIdade)));

        maisVelho.ifPresent(p -> System.out.println("Mais velho: " + p.getNome()));
        maisNovo.ifPresent(p -> System.out.println("Mais novo: " + p.getNome()));

        // Soma das idades
        Integer somaIdades = pessoas.stream()
                .collect(Collectors.summingInt(Pessoa::getIdade));
        System.out.println("Soma das idades: " + somaIdades);

        // Coletando para coleções específicas
        System.out.println("\n=== COLETANDO PARA COLEÇÕES ESPECÍFICAS ===");

        TreeSet<String> nomesOrdenados = pessoas.stream()
                .map(Pessoa::getNome)
                .collect(Collectors.toCollection(TreeSet::new));
        System.out.println("Nomes ordenados: " + nomesOrdenados);

        // Operações paralelas
        System.out.println("\n=== STREAMS PARALELAS ===");

        List<String> nomesParalelo = pessoas.parallelStream()
                                           .map(Pessoa::getNome)
                                           .collect(Collectors.toList());
        System.out.println("Processamento paralelo: " + nomesParalelo);

        // Benchmarking sequencial vs paralelo
        long inicio = System.currentTimeMillis();
        List<String> sequencial = pessoas.stream()
                                        .map(p -> {
                                            try { Thread.sleep(10); } catch (Exception e) {}
                                            return p.getNome().toUpperCase();
                                        })
                                        .collect(Collectors.toList());
        long fimSequencial = System.currentTimeMillis();

        long inicioParalelo = System.currentTimeMillis();
        List<String> paralelo = pessoas.parallelStream()
                                      .map(p -> {
                                          try { Thread.sleep(10); } catch (Exception e) {}
                                          return p.getNome().toUpperCase();
                                      })
                                      .collect(Collectors.toList());
        long fimParalelo = System.currentTimeMillis();

        System.out.printf("Tempo sequencial: %dms\n", fimSequencial - inicio);
        System.out.printf("Tempo paralelo: %dms\n", fimParalelo - inicioParalelo);
    }
}
```

### **9.2.6 Streams API - Casos de Uso Avançados**

**Exemplo 9.6: Casos de Uso Avançados com Streams**

```java
import java.util.*;
import java.util.stream.*;
import java.nio.file.*;
import java.io.IOException;

public class ExemploStreamsAvancado {

    static class Transacao {
        private String id;
        private String tipo; // "COMPRA", "VENDA"
        private double valor;
        private String moeda;
        private Date data;

        public Transacao(String id, String tipo, double valor, String moeda, Date data) {
            this.id = id;
            this.tipo = tipo;
            this.valor = valor;
            this.moeda = moeda;
            this.data = data;
        }

        // Getters
        public String getId() { return id; }
        public String getTipo() { return tipo; }
        public double getValor() { return valor; }
        public String getMoeda() { return moeda; }
        public Date getData() { return data; }

        @Override
        public String toString() {
            return String.format("Transacao{id='%s', tipo='%s', valor=%.2f, moeda='%s', data=%s}",
                    id, tipo, valor, moeda, data);
        }
    }

    public static void main(String[] args) {
        System.out.println("=== CASOS DE USO AVANÇADOS COM STREAMS ===");

        List<Transacao> transacoes = Arrays.asList(
            new Transacao("T1", "COMPRA", 1000.00, "USD", new Date()),
            new Transacao("T2", "VENDA", 500.00, "USD", new Date()),
            new Transacao("T3", "COMPRA", 2000.00, "EUR", new Date()),
            new Transacao("T4", "COMPRA", 1500.00, "USD", new Date()),
            new Transacao("T5", "VENDA", 800.00, "EUR", new Date()),
            new Transacao("T6", "COMPRA", 3000.00, "BRL", new Date()),
            new Transacao("T7", "VENDA", 1200.00, "USD", new Date())
        );

        // Análise financeira
        System.out.println("\n=== ANÁLISE FINANCEIRA ===");

        // Total de compras por moeda
        Map<String, Double> comprasPorMoeda = transacoes.stream()
                .filter(t -> "COMPRA".equals(t.getTipo()))
                .collect(Collectors.groupingBy(
                    Transacao::getMoeda,
                    Collectors.summingDouble(Transacao::getValor)
                ));
        System.out.println("Compras por moeda: " + comprasPorMoeda);

        // Top 3 transações mais altas
        System.out.println("\nTop 3 transações mais altas:");
        transacoes.stream()
                 .sorted(Comparator.comparing(Transacao::getValor).reversed())
                 .limit(3)
                 .forEach(t -> System.out.printf("%s: %.2f %s\n", 
                         t.getId(), t.getValor(), t.getMoeda()));

        // Valor total por tipo e moeda
        Map<String, Map<String, Double>> resumo = transacoes.stream()
                .collect(Collectors.groupingBy(
                    Transacao::getTipo,
                    Collectors.groupingBy(
                        Transacao::getMoeda,
                        Collectors.summingDouble(Transacao::getValor)
                    )
                ));
        System.out.println("\nResumo por tipo e moeda: " + resumo);

        // Processamento de arquivos com Streams
        System.out.println("\n=== PROCESSAMENTO DE ARQUIVOS ===");

        try {
            // Ler arquivo e processar linhas
            Path arquivo = Paths.get("dados.txt");
            
            // Se o arquivo existir, processá-lo
            if (Files.exists(arquivo)) {
                List<String> linhas = Files.lines(arquivo)
                                          .collect(Collectors.toList());

                // Estatísticas das linhas
                LongSummaryStatistics statsLinhas = linhas.stream()
                        .mapToLong(String::length)
                        .summaryStatistics();

                System.out.println("Estatísticas do arquivo:");
                System.out.printf("Total linhas: %d\n", linhas.size());
                System.out.printf("Maior linha: %d chars\n", statsLinhas.getMax());
                System.out.printf("Menor linha: %d chars\n", statsLinhas.getMin());
                System.out.printf("Média: %.1f chars\n", statsLinhas.getAverage());

                // Palavras mais frequentes
                Map<String, Long> frequenciaPalavras = linhas.stream()
                        .flatMap(linha -> Arrays.stream(linha.split("\\s+")))
                        .map(String::toLowerCase)
                        .filter(palavra -> palavra.length() > 3)
                        .collect(Collectors.groupingBy(
                            palavra -> palavra,
                            Collectors.counting()
                        ));

                System.out.println("\nPalavras mais frequentes:");
                frequenciaPalavras.entrySet().stream()
                                 .sorted(Map.Entry.<String, Long>comparingByValue().reversed())
                                 .limit(5)
                                 .forEach(entry -> 
                                     System.out.printf("%s: %d\n", entry.getKey(), entry.getValue()));
            }
        } catch (IOException e) {
            System.out.println("Erro ao processar arquivo: " + e.getMessage());
        }

        // Streams com Optional
        System.out.println("\n=== STREAMS COM OPTIONAL ===");

        Optional<Transacao> transacaoMaisCara = transacoes.stream()
                .max(Comparator.comparing(Transacao::getValor));

        transacaoMaisCara.ifPresent(t -> 
            System.out.println("Transação mais cara: " + t.getValor()));

        // Encadeamento de Optionals
        String resultado = transacaoMaisCara
                .map(Transacao::getMoeda)
                .filter(moeda -> moeda.equals("USD"))
                .map(moeda -> "Moeda: " + moeda)
                .orElse("Moeda não encontrada");

        System.out.println("Resultado: " + resultado);

        // Streams infinitas para geração de dados
        System.out.println("\n=== STREAMS INFINITAS ===");

        // Gerar sequência Fibonacci
        System.out.println("Fibonacci (10 primeiros):");
        Stream.iterate(new long[]{0, 1}, fib -> new long[]{fib[1], fib[0] + fib[1]})
              .limit(10)
              .mapToLong(fib -> fib[0])
              .forEach(fib -> System.out.print(fib + " "));

        // Números aleatórios
        System.out.println("\n\nNúmeros aleatórios (5):");
        new Random().doubles(5, 0, 100)
                   .forEach(d -> System.out.printf("%.2f ", d));

        // Custom Collector
        System.out.println("\n\n=== CUSTOM COLLECTOR ===");

        Collector<Transacao, ?, Map<String, List<Transacao>>> collectorPorMoeda = 
            Collector.of(
                HashMap::new, // supplier
                (map, transacao) -> {
                    map.computeIfAbsent(transacao.getMoeda(), k -> new ArrayList<>())
                       .add(transacao);
                }, // accumulator
                (map1, map2) -> {
                    map2.forEach((moeda, transacoes) -> {
                        map1.computeIfAbsent(moeda, k -> new ArrayList<>())
                            .addAll(transacoes);
                    });
                    return map1;
                }, // combiner (para paralelo)
                Collector.Characteristics.IDENTITY_FINISH
            );

        Map<String, List<Transacao>> transacoesPorMoeda = transacoes.stream()
                                                                   .collect(collectorPorMoeda);
        System.out.println("Transações por moeda (custom collector): " + transacoesPorMoeda);
    }
}
```

## **9.3 Exercícios Práticos**

### **Exercício 9.1: Processador de Texto com Streams**

```java
import java.util.*;
import java.util.stream.*;

public class ProcessadorTexto {

    public static Map<String, Long> contarPalavras(String texto) {
        if (texto == null || texto.trim().isEmpty()) {
            return Collections.emptyMap();
        }

        return Arrays.stream(texto.toLowerCase().split("\\W+"))
                    .filter(palavra -> !palavra.isEmpty())
                    .collect(Collectors.groupingBy(
                        palavra -> palavra,
                        Collectors.counting()
                    ));
    }

    public static List<String> palavrasMaisFrequentes(String texto, int limite) {
        Map<String, Long> contagem = contarPalavras(texto);

        return contagem.entrySet().stream()
                      .sorted(Map.Entry.<String, Long>comparingByValue().reversed())
                      .limit(limite)
                      .map(Map.Entry::getKey)
                      .collect(Collectors.toList());
    }

    public static Map<Integer, List<String>> palavrasPorTamanho(String texto) {
        if (texto == null || texto.trim().isEmpty()) {
            return Collections.emptyMap();
        }

        return Arrays.stream(texto.toLowerCase().split("\\W+"))
                    .filter(palavra -> !palavra.isEmpty())
                    .collect(Collectors.groupingBy(
                        String::length,
                        Collectors.toList()
                    ));
    }

    public static EstatisticasTexto analisarTexto(String texto) {
        if (texto == null) {
            return new EstatisticasTexto(0, 0, 0, 0, 0, Collections.emptyMap());
        }

        String[] palavras = texto.split("\\W+");
        String[] frases = texto.split("[.!?]+");

        long numeroPalavras = Arrays.stream(palavras)
                                   .filter(palavra -> !palavra.isEmpty())
                                   .count();

        long numeroFrases = Arrays.stream(frases)
                                 .filter(frase -> !frase.trim().isEmpty())
                                 .count();

        long numeroCaracteres = texto.length();
        long numeroCaracteresSemEspaco = texto.replaceAll("\\s", "").length();
        long numeroLinhas = texto.split("\r\n|\r|\n").length;

        Map<String, Long> palavrasFrequentes = contarPalavras(texto);

        return new EstatisticasTexto(
            numeroPalavras, numeroFrases, numeroCaracteres,
            numeroCaracteresSemEspaco, numeroLinhas, palavrasFrequentes
        );
    }

    static class EstatisticasTexto {
        private final long numeroPalavras;
        private final long numeroFrases;
        private final long numeroCaracteres;
        private final long numeroCaracteresSemEspaco;
        private final long numeroLinhas;
        private final Map<String, Long> palavrasFrequentes;

        public EstatisticasTexto(long numeroPalavras, long numeroFrases, 
                                long numeroCaracteres, long numeroCaracteresSemEspaco,
                                long numeroLinhas, Map<String, Long> palavrasFrequentes) {
            this.numeroPalavras = numeroPalavras;
            this.numeroFrases = numeroFrases;
            this.numeroCaracteres = numeroCaracteres;
            this.numeroCaracteresSemEspaco = numeroCaracteresSemEspaco;
            this.numeroLinhas = numeroLinhas;
            this.palavrasFrequentes = palavrasFrequentes;
        }

        @Override
        public String toString() {
            return String.format(
                "EstatisticasTexto{palavras=%d, frases=%d, caracteres=%d, caracteresSemEspaco=%d, linhas=%d}",
                numeroPalavras, numeroFrases, numeroCaracteres, numeroCaracteresSemEspaco, numeroLinhas
            );
        }
    }

    public static void main(String[] args) {
        String textoExemplo = 
            "Java é uma linguagem de programação. Java é popular e poderosa. " +
            "Programação em Java é divertida. Java é usada em muitos projetos. " +
            "Aprender Java é importante para desenvolvedores. Desenvolvimento com Java é eficiente.";

        System.out.println("=== PROCESSADOR DE TEXTO COM STREAMS ===");

        // Contagem de palavras
        Map<String, Long> contagem = contarPalavras(textoExemplo);
        System.out.println("Contagem de palavras: " + contagem);

        // Palavras mais frequentes
        List<String> maisFrequentes = palavrasMaisFrequentes(textoExemplo, 5);
        System.out.println("5 palavras mais frequentes: " + maisFrequentes);

        // Palavras por tamanho
        Map<Integer, List<String>> porTamanho = palavrasPorTamanho(textoExemplo);
        System.out.println("Palavras por tamanho: " + porTamanho);

        // Estatísticas completas
        EstatisticasTexto stats = analisarTexto(textoExemplo);
        System.out.println("Estatísticas: " + stats);

        // Análise detalhada das palavras frequentes
        System.out.println("\nDetalhes das palavras frequentes:");
        contagem.entrySet().stream()
               .sorted(Map.Entry.<String, Long>comparingByValue().reversed())
               .forEach(entry -> 
                   System.out.printf("'%s': %d ocorrências\n", entry.getKey(), entry.getValue()));
    }
}
```

### **Exercício 9.2: Sistema de Análise de Vendas**

```java
import java.util.*;
import java.util.stream.*;

public class AnaliseVendas {

    static class Venda {
        private String id;
        private String vendedor;
        private String produto;
        private int quantidade;
        private double valorUnitario;
        private Date data;
        private String regiao;

        public Venda(String id, String vendedor, String produto, int quantidade, 
                    double valorUnitario, Date data, String regiao) {
            this.id = id;
            this.vendedor = vendedor;
            this.produto = produto;
            this.quantidade = quantidade;
            this.valorUnitario = valorUnitario;
            this.data = data;
            this.regiao = regiao;
        }

        public double getValorTotal() {
            return quantidade * valorUnitario;
        }

        // Getters
        public String getId() { return id; }
        public String getVendedor() { return vendedor; }
        public String getProduto() { return produto; }
        public int getQuantidade() { return quantidade; }
        public double getValorUnitario() { return valorUnitario; }
        public Date getData() { return data; }
        public String getRegiao() { return regiao; }
    }

    public static class AnalisadorVendas {
        private List<Venda> vendas;

        public AnalisadorVendas(List<Venda> vendas) {
            this.vendas = vendas;
        }

        // 1. Total de vendas
        public double getTotalVendas() {
            return vendas.stream()
                        .mapToDouble(Venda::getValorTotal)
                        .sum();
        }

        // 2. Média de valor por venda
        public double getMediaValorVenda() {
            return vendas.stream()
                        .mapToDouble(Venda::getValorTotal)
                        .average()
                        .orElse(0.0);
        }

        // 3. Venda mais valiosa
        public Optional<Venda> getVendaMaisValiosa() {
            return vendas.stream()
                        .max(Comparator.comparing(Venda::getValorTotal));
        }

        // 4. Vendas por vendedor
        public Map<String, Double> getVendasPorVendedor() {
            return vendas.stream()
                        .collect(Collectors.groupingBy(
                            Venda::getVendedor,
                            Collectors.summingDouble(Venda::getValorTotal)
                        ));
        }

        // 5. Vendas por produto
        public Map<String, Double> getVendasPorProduto() {
            return vendas.stream()
                        .collect(Collectors.groupingBy(
                            Venda::getProduto,
                            Collectors.summingDouble(Venda::getValorTotal)
                        ));
        }

        // 6. Vendas por região
        public Map<String, Double> getVendasPorRegiao() {
            return vendas.stream()
                        .collect(Collectors.groupingBy(
                            Venda::getRegiao,
                            Collectors.summingDouble(Venda::getValorTotal)
                        ));
        }

        // 7. Top N vendedores
        public List<Map.Entry<String, Double>> getTopVendedores(int n) {
            return getVendasPorVendedor().entrySet().stream()
                    .sorted(Map.Entry.<String, Double>comparingByValue().reversed())
                    .limit(n)
                    .collect(Collectors.toList());
        }

        // 8. Produtos mais vendidos (quantidade)
        public Map<String, Integer> getProdutosMaisVendidos() {
            return vendas.stream()
                        .collect(Collectors.groupingBy(
                            Venda::getProduto,
                            Collectors.summingInt(Venda::getQuantidade)
                        ));
        }

        // 9. Estatísticas de quantidade
        public IntSummaryStatistics getEstatisticasQuantidade() {
            return vendas.stream()
                        .mapToInt(Venda::getQuantidade)
                        .summaryStatistics();
        }

        // 10. Vendas agrupadas por região e produto
        public Map<String, Map<String, Double>> getVendasPorRegiaoEProduto() {
            return vendas.stream()
                        .collect(Collectors.groupingBy(
                            Venda::getRegiao,
                            Collectors.groupingBy(
                                Venda::getProduto,
                                Collectors.summingDouble(Venda::getValorTotal)
                            )
                        ));
        }

        // 11. Vendas com valor acima da média
        public List<Venda> getVendasAcimaMedia() {
            double media = getMediaValorVenda();
            return vendas.stream()
                        .filter(venda -> venda.getValorTotal() > media)
                        .collect(Collectors.toList());
        }

        // 12. Resumo completo
        public void imprimirResumo() {
            System.out.println("=== RESUMO DE VENDAS ===");
            System.out.printf("Total de vendas: R$%.2f\n", getTotalVendas());
            System.out.printf("Média por venda: R$%.2f\n", getMediaValorVenda());
            System.out.printf("Total de transações: %d\n", vendas.size());

            getVendaMaisValiosa().ifPresent(v -> 
                System.out.printf("Venda mais valiosa: %s - R$%.2f\n", 
                    v.getId(), v.getValorTotal()));

            System.out.println("\nVendas por vendedor:");
            getVendasPorVendedor().forEach((vendedor, total) -> 
                System.out.printf("  %s: R$%.2f\n", vendedor, total));

            System.out.println("\nTop 3 vendedores:");
            getTopVendedores(3).forEach(entry -> 
                System.out.printf("  %s: R$%.2f\n", entry.getKey(), entry.getValue()));

            System.out.println("\nEstatísticas de quantidade:");
            IntSummaryStatistics stats = getEstatisticasQuantidade();
            System.out.printf("  Média: %.1f, Min: %d, Max: %d, Total: %d\n",
                    stats.getAverage(), stats.getMin(), stats.getMax(), stats.getSum());
        }
    }

    public static void main(String[] args) {
        // Criando dados de exemplo
        List<Venda> vendas = Arrays.asList(
            new Venda("V001", "João", "Notebook", 2, 2500.00, new Date(), "Sudeste"),
            new Venda("V002", "Maria", "Mouse", 10, 50.00, new Date(), "Sul"),
            new Venda("V003", "João", "Teclado", 5, 150.00, new Date(), "Sudeste"),
            new Venda("V004", "Pedro", "Monitor", 3, 800.00, new Date(), "Nordeste"),
            new Venda("V005", "Maria", "Notebook", 1, 2500.00, new Date(), "Sul"),
            new Venda("V006", "Ana", "Headphone", 8, 200.00, new Date(), "Sudeste"),
            new Venda("V007", "João", "Monitor", 2, 800.00, new Date(), "Sudeste"),
            new Venda("V008", "Pedro", "Mouse", 15, 50.00, new Date(), "Nordeste"),
            new Venda("V009", "Ana", "Teclado", 4, 150.00, new Date(), "Sul"),
            new Venda("V010", "Maria", "Headphone", 6, 200.00, new Date(), "Sul")
        );

        AnalisadorVendas analisador = new AnalisadorVendas(vendas);

        // Relatórios
        analisador.imprimirResumo();

        // Análises adicionais
        System.out.println("\n=== ANÁLISES DETALHADAS ===");

        System.out.println("Vendas por região:");
        analisador.getVendasPorRegiao().forEach((regiao, total) -> 
            System.out.printf("  %s: R$%.2f\n", regiao, total));

        System.out.println("\nVendas por região e produto:");
        analisador.getVendasPorRegiaoEProduto().forEach((regiao, produtos) -> {
            System.out.println("  " + regiao + ":");
            produtos.forEach((produto, total) -> 
                System.out.printf("    %s: R$%.2f\n", produto, total));
        });

        System.out.println("\nProdutos mais vendidos (quantidade):");
        analisador.getProdutosMaisVendidos().entrySet().stream()
                 .sorted(Map.Entry.<String, Integer>comparingByValue().reversed())
                 .forEach(entry -> 
                     System.out.printf("  %s: %d unidades\n", entry.getKey(), entry.getValue()));

        System.out.println("\nVendas acima da média:");
        analisador.getVendasAcimaMedia().forEach(venda -> 
            System.out.printf("  %s: R$%.2f\n", venda.getId(), venda.getValorTotal()));
    }
}
```

## **9.4 Caso Prático: Sistema de Recomendação Simples**

```java
import java.util.*;
import java.util.stream.*;
import java.util.function.*;

public class SistemaRecomendacao {

    static class Usuario {
        private String id;
        private String nome;
        private Set<String> interesses;

        public Usuario(String id, String nome, Set<String> interesses) {
            this.id = id;
            this.nome = nome;
            this.interesses = interesses;
        }

        public String getId() { return id; }
        public String getNome() { return nome; }
        public Set<String> getInteresses() { return interesses; }
    }

    static class Produto {
        private String id;
        private String nome;
        private String categoria;
        private Set<String> tags;
        private double preco;
        private int vendas;

        public Produto(String id, String nome, String categoria, Set<String> tags, double preco, int vendas) {
            this.id = id;
            this.nome = nome;
            this.categoria = categoria;
            this.tags = tags;
            this.preco = preco;
            this.vendas = vendas;
        }

        public String getId() { return id; }
        public String getNome() { return nome; }
        public String getCategoria() { return categoria; }
        public Set<String> getTags() { return tags; }
        public double getPreco() { return preco; }
        public int getVendas() { return vendas; }
    }

    static class Recomendacao {
        private Produto produto;
        private double score;

        public Recomendacao(Produto produto, double score) {
            this.produto = produto;
            this.score = score;
        }

        public Produto getProduto() { return produto; }
        public double getScore() { return score; }

        @Override
        public String toString() {
            return String.format("Recomendacao{produto=%s, score=%.2f}", produto.getNome(), score);
        }
    }

    public static class MotorRecomendacao {
        private List<Usuario> usuarios;
        private List<Produto> produtos;

        public MotorRecomendacao(List<Usuario> usuarios, List<Produto> produtos) {
            this.usuarios = usuarios;
            this.produtos = produtos;
        }

        // 1. Recomendação baseada em interesses
        public List<Recomendacao> recomendarPorInteresses(Usuario usuario, int limite) {
            Set<String> interessesUsuario = usuario.getInteresses();

            return produtos.stream()
                          .map(produto -> {
                              double score = calcularScoreInteresse(interessesUsuario, produto.getTags());
                              return new Recomendacao(produto, score);
                          })
                          .sorted(Comparator.comparing(Recomendacao::getScore).reversed())
                          .limit(limite)
                          .collect(Collectors.toList());
        }

        private double calcularScoreInteresse(Set<String> interesses, Set<String> tagsProduto) {
            long matches = interesses.stream()
                                   .filter(tagsProduto::contains)
                                   .count();
            return (double) matches / interesses.size();
        }

        // 2. Recomendação baseada em popularidade
        public List<Recomendacao> recomendarPorPopularidade(int limite) {
            return produtos.stream()
                          .sorted(Comparator.comparing(Produto::getVendas).reversed())
                          .limit(limite)
                          .map(produto -> new Recomendacao(produto, produto.getVendas()))
                          .collect(Collectors.toList());
        }

        // 3. Recomendação baseada em categoria
        public List<Recomendacao> recomendarPorCategoria(String categoria, int limite) {
            return produtos.stream()
                          .filter(produto -> produto.getCategoria().equals(categoria))
                          .sorted(Comparator.comparing(Produto::getVendas).reversed())
                          .limit(limite)
                          .map(produto -> new Recomendacao(produto, produto.getVendas()))
                          .collect(Collectors.toList());
        }

        // 4. Recomendação híbrida
        public List<Recomendacao> recomendarHibrido(Usuario usuario, int limite) {
            // Combina score de interesse com popularidade
            return produtos.stream()
                          .map(produto -> {
                              double scoreInteresse = calcularScoreInteresse(
                                  usuario.getInteresses(), produto.getTags());
                              double scorePopularidade = normalizarPopularidade(produto.getVendas());
                              double scoreFinal = (scoreInteresse * 0.7) + (scorePopularidade * 0.3);
                              return new Recomendacao(produto, scoreFinal);
                          })
                          .sorted(Comparator.comparing(Recomendacao::getScore).reversed())
                          .limit(limite)
                          .collect(Collectors.toList());
        }

        private double normalizarPopularidade(int vendas) {
            int maxVendas = produtos.stream()
                                   .mapToInt(Produto::getVendas)
                                   .max()
                                   .orElse(1);
            return (double) vendas / maxVendas;
        }

        // 5. Produtos similares
        public List<Recomendacao> encontrarSimilares(Produto produtoAlvo, int limite) {
            return produtos.stream()
                          .filter(produto -> !produto.getId().equals(produtoAlvo.getId()))
                          .map(produto -> {
                              double similaridade = calcularSimilaridade(produtoAlvo.getTags(), produto.getTags());
                              return new Recomendacao(produto, similaridade);
                          })
                          .sorted(Comparator.comparing(Recomendacao::getScore).reversed())
                          .limit(limite)
                          .collect(Collectors.toList());
        }

        private double calcularSimilaridade(Set<String> tags1, Set<String> tags2) {
            Set<String> uniao = new HashSet<>(tags1);
            uniao.addAll(tags2);

            Set<String> interseccao = new HashSet<>(tags1);
            interseccao.retainAll(tags2);

            return (double) interseccao.size() / uniao.size();
        }

        // 6. Análise de usuários similares
        public List<Usuario> encontrarUsuariosSimilares(Usuario usuarioAlvo, int limite) {
            return usuarios.stream()
                          .filter(usuario -> !usuario.getId().equals(usuarioAlvo.getId()))
                          .map(usuario -> {
                              double similaridade = calcularSimilaridade(
                                  usuarioAlvo.getInteresses(), usuario.getInteresses());
                              return new AbstractMap.SimpleEntry<>(usuario, similaridade);
                          })
                          .sorted(Map.Entry.<Usuario, Double>comparingByValue().reversed())
                          .limit(limite)
                          .map(Map.Entry::getKey)
                          .collect(Collectors.toList());
        }
    }

    public static void main(String[] args) {
        // Dados de exemplo
        Usuario usuario1 = new Usuario("U1", "Alice", Set.of("tecnologia", "programação", "java", "web"));
        Usuario usuario2 = new Usuario("U2", "Bob", Set.of("games", "hardware", "tecnologia"));
        Usuario usuario3 = new Usuario("U3", "Charlie", Set.of("livros", "musica", "arte"));

        List<Usuario> usuarios = Arrays.asList(usuario1, usuario2, usuario3);

        List<Produto> produtos = Arrays.asList(
            new Produto("P1", "Java Programming", "Livros", 
                       Set.of("java", "programação", "tecnologia"), 80.00, 150),
            new Produto("P2", "Gaming Mouse", "Hardware", 
                       Set.of("games", "hardware", "tecnologia"), 120.00, 200),
            new Produto("P3", "Web Development", "Livros", 
                       Set.of("web", "programação", "tecnologia"), 70.00, 100),
            new Produto("P4", "Noise Cancelling Headphones", "Áudio", 
                       Set.of("musica", "tecnologia"), 250.00, 80),
            new Produto("P5", "Art History", "Livros", 
                       Set.of("arte", "livros", "história"), 60.00, 50),
            new Produto("P6", "Mechanical Keyboard", "Hardware", 
                       Set.of("hardware", "tecnologia", "games"), 180.00, 120)
        );

        MotorRecomendacao motor = new MotorRecomendacao(usuarios, produtos);

        System.out.println("=== SISTEMA DE RECOMENDAÇÃO ===");

        // Recomendações para Alice
        System.out.println("\nRecomendações para Alice (por interesses):");
        motor.recomendarPorInteresses(usuario1, 3).forEach(System.out::println);

        System.out.println("\nRecomendações para Alice (híbrido):");
        motor.recomendarHibrido(usuario1, 3).forEach(System.out::println);

        // Produtos populares
        System.out.println("\nProdutos populares:");
        motor.recomendarPorPopularidade(3).forEach(System.out::println);

        // Produtos similares
        System.out.println("\nProdutos similares a 'Java Programming':");
        Produto javaBook = produtos.get(0);
        motor.encontrarSimilares(javaBook, 3).forEach(System.out::println);

        // Usuários similares
        System.out.println("\nUsuários similares a Alice:");
        motor.encontrarUsuariosSimilares(usuario1, 2).forEach(usuario -> 
            System.out.println(usuario.getNome()));

        // Análise de categorias
        System.out.println("\nRecomendações de Livros:");
        motor.recomendarPorCategoria("Livros", 5).forEach(System.out::println);
    }
}
```

## **9.5 Questionário de Revisão**

**Questão 1:** Qual é a principal característica de uma expressão lambda?
- A) É uma função anônima que pode ser passada como parâmetro
- B) É um método estático de uma classe
- C) É uma interface com múltiplos métodos

**Questão 2:** O que é uma interface funcional?
- A) Interface com apenas um método abstrato
- B) Interface que implementa funções matemáticas
- C) Interface com métodos default

**Questão 3:** Qual a diferença entre `map` e `flatMap` em Streams?
- A) `map` transforma 1-para-1, `flatMap` transforma 1-para-muitos
- B) `map` é para operações matemáticas, `flatMap` para strings
- C) `map` é mais rápido que `flatMap`

**Questão 4:** Qual operação terminal retorna `Optional<T>`?
- A) `findFirst()`
- B) `forEach()`
- C) `count()`

**Questão 5:** O que significa "lazy evaluation" em Streams?
- A) Operações intermediárias só são executadas quando necessário
- B) Streams são lentas por natureza
- C) Operações são executadas em background

## **9.6 Laboratório Prático**

**Projeto: Analisador de Dados de Rede Social**

```java
// Implemente um sistema que analise dados de uma rede social:
// 1. Calcular estatísticas de usuários (idade, localização, etc.)
// 2. Encontrar usuários mais influentes
// 3. Analisar relacionamentos e comunidades
// 4. Recomendar conexões
// 5. Identificar tópicos populares

// Use: Streams, Lambda, Method References, Collectors
```

## **9.7 Material de Apoio**

**Resumo das Principais Interfaces Funcionais:**

- **Predicate<T>**: `boolean test(T t)` - filtros
- **Function<T,R>**: `R apply(T t)` - transformações
- **Consumer<T>**: `void accept(T t)` - consumidores
- **Supplier<T>**: `T get()` - fornecedores
- **UnaryOperator<T>**: `T apply(T t)` - função identidade

**Operações Intermediárias Comuns:**
- `filter(Predicate)`: filtra elementos
- `map(Function)`: transforma elementos
- `flatMap(Function)`: transforma e achata
- `distinct()`: remove duplicatas
- `sorted()`: ordena elementos
- `peek(Consumer)`: debug ou side-effects

**Operações Terminais Comuns:**
- `forEach(Consumer)`: itera sobre elementos
- `collect(Collector)`: coleta em coleção
- `toArray()`: converte para array
- `reduce()`: redução personalizada
- `count()`: conta elementos
- `anyMatch()/allMatch()/noneMatch()`: testes

**Collectors Úteis:**
- `toList()`, `toSet()`, `toMap()`
- `groupingBy()`: agrupamento
- `partitioningBy()`: divisão binária
- `joining()`: concatena strings
- `summarizingInt()`: estatísticas

**Dicas de Performance:**
- Use `parallelStream()` para processamento paralelo
- Prefira operações stateless
- Evite side-effects em operações intermediárias
- Use `findFirst()` em vez de `limit(1).findAny()`

---

**Próximo Módulo: Tratamento de Exceções e Assertions**

Preparado para explorar o robusto sistema de tratamento de exceções do Java?

---

# **Módulo 10: Tratamento de Exceções e Assertions**

## **10.1 Objetivos do Módulo**

- Compreender a hierarquia de exceções em Java
- Dominar o uso de try-catch-finally para tratamento de exceções
- Aprender a criar e usar exceções personalizadas
- Conhecer as melhores práticas de tratamento de exceções
- Aprender a usar assertions para verificação de invariantes
- Entender a diferença entre exceções verificadas e não verificadas

## **10.2 Conteúdo Programático**

### **10.2.1 Fundamentos de Exceções**

**Exemplo 10.1: Hierarquia e Tipos de Exceções**

```java
import java.io.*;
import java.util.*;

public class ExemploHierarquiaExcecoes {

    public static void main(String[] args) {
        System.out.println("=== HIERARQUIA DE EXCEÇÕES ===");

        // Throwable é a classe raiz
        System.out.println("Throwable");
        System.out.println("├── Error (erros graves do sistema)");
        System.out.println("└── Exception");
        System.out.println("    ├── RuntimeException (Unchecked)");
        System.out.println("    └── Outras Exceções (Checked)");

        // Exceções Verificadas (Checked): devem ser tratadas ou declaradas
        // Exceções Não Verificadas (Unchecked): RuntimeException e Error

        demonstrarExcecoesComuns();
        demonstrarExcecoesVerificadas();
    }

    public static void demonstrarExcecoesComuns() {
        System.out.println("\n=== EXCEÇÕES NÃO VERIFICADAS (UNCHECKED) ===");

        // NullPointerException
        try {
            String str = null;
            System.out.println(str.length());
        } catch (NullPointerException e) {
            System.out.println("NullPointerException: " + e.getMessage());
        }

        // ArrayIndexOutOfBoundsException
        try {
            int[] array = new int[5];
            array[10] = 50;
        } catch (ArrayIndexOutOfBoundsException e) {
            System.out.println("ArrayIndexOutOfBoundsException: " + e.getMessage());
        }

        // NumberFormatException
        try {
            int numero = Integer.parseInt("abc");
        } catch (NumberFormatException e) {
            System.out.println("NumberFormatException: " + e.getMessage());
        }

        // ClassCastException
        try {
            Object obj = "String";
            Integer inteiro = (Integer) obj;
        } catch (ClassCastException e) {
            System.out.println("ClassCastException: " + e.getMessage());
        }

        // ArithmeticException
        try {
            int resultado = 10 / 0;
        } catch (ArithmeticException e) {
            System.out.println("ArithmeticException: " + e.getMessage());
        }

        // IllegalArgumentException
        try {
            throw new IllegalArgumentException("Argumento inválido");
        } catch (IllegalArgumentException e) {
            System.out.println("IllegalArgumentException: " + e.getMessage());
        }
    }

    public static void demonstrarExcecoesVerificadas() {
        System.out.println("\n=== EXCEÇÕES VERIFICADAS (CHECKED) ===");

        // IOException
        try {
            FileReader reader = new FileReader("arquivo_inexistente.txt");
        } catch (FileNotFoundException e) {
            System.out.println("FileNotFoundException: " + e.getMessage());
        }

        // ParseException (precisa ser importada)
        try {
            throw new java.text.ParseException("Erro de parsing", 0);
        } catch (java.text.ParseException e) {
            System.out.println("ParseException: " + e.getMessage());
        }

        // InterruptedException
        try {
            Thread.sleep(1000);
            Thread.currentThread().interrupt();
            Thread.sleep(1000); // Vai lançar InterruptedException
        } catch (InterruptedException e) {
            System.out.println("InterruptedException: " + e.getMessage());
            Thread.currentThread().interrupt(); // Restaurar o status de interrupção
        }
    }
}
```

### **10.2.2 Try-Catch-Finally**

**Exemplo 10.2: Tratamento de Exceções com Try-Catch-Finally**

```java
import java.io.*;
import java.util.*;

public class ExemploTryCatchFinally {

    public static void main(String[] args) {
        System.out.println("=== TRY-CATCH-FINALLY ===");

        // Exemplo básico
        try {
            int resultado = 10 / 0;
            System.out.println("Resultado: " + resultado);
        } catch (ArithmeticException e) {
            System.out.println("Erro aritmético: " + e.getMessage());
        } finally {
            System.out.println("Bloco finally sempre executado");
        }

        // Múltiplos catch
        try {
            String str = null;
            int numero = Integer.parseInt(str);
        } catch (NullPointerException e) {
            System.out.println("NullPointerException: " + e.getMessage());
        } catch (NumberFormatException e) {
            System.out.println("NumberFormatException: " + e.getMessage());
        } catch (Exception e) {
            System.out.println("Exception genérica: " + e.getMessage());
        } finally {
            System.out.println("Finally após múltiplos catch");
        }

        // Try com recursos (Java 7+)
        tryWithResources();

        // Capturando múltiplas exceções em um bloco (Java 7+)
        capturarMultiplasExcecoes();

        // Finally com retorno
        testarFinallyComRetorno();
    }

    public static void tryWithResources() {
        System.out.println("\n=== TRY-WITH-RESOURCES ===");

        // Recursos que implementam AutoCloseable são fechados automaticamente
        try (Scanner scanner = new Scanner(new File("arquivo_inexistente.txt"))) {
            while (scanner.hasNext()) {
                System.out.println(scanner.nextLine());
            }
        } catch (FileNotFoundException e) {
            System.out.println("Arquivo não encontrado: " + e.getMessage());
        }
        // Scanner é fechado automaticamente, não precisa de finally

        // Múltiplos recursos
        try (FileInputStream input = new FileInputStream("entrada.txt");
             FileOutputStream output = new FileOutputStream("saida.txt")) {
            
            byte[] buffer = new byte[1024];
            int bytesLidos;
            while ((bytesLidos = input.read(buffer)) != -1) {
                output.write(buffer, 0, bytesLidos);
            }
        } catch (IOException e) {
            System.out.println("Erro de I/O: " + e.getMessage());
        }
    }

    public static void capturarMultiplasExcecoes() {
        System.out.println("\n=== CAPTURANDO MÚLTIPLAS EXCEÇÕES ===");

        try {
            // Código que pode lançar diferentes exceções
            String[] array = new String[5];
            array[10] = "valor"; // Pode lançar ArrayIndexOutOfBoundsException
            int numero = Integer.parseInt(array[10]); // Pode lançar NumberFormatException
        } catch (ArrayIndexOutOfBoundsException | NumberFormatException e) {
            System.out.println("Exceção capturada: " + e.getClass().getSimpleName());
            System.out.println("Mensagem: " + e.getMessage());
        }
    }

    public static void testarFinallyComRetorno() {
        System.out.println("\n=== FINALLY COM RETURN ===");

        System.out.println("Valor retornado: " = metodoComFinally());
    }

    public static String metodoComFinally() {
        try {
            System.out.println("No bloco try");
            return "Retorno do try";
        } catch (Exception e) {
            System.out.println("No bloco catch");
            return "Retorno do catch";
        } finally {
            System.out.println("No bloco finally - executado antes do return");
        }
    }
}
```

### **10.2.3 Lançamento de Exceções**

**Exemplo 10.3: Lançando e Propagando Exceções**

```java
import java.io.*;
import java.util.*;

public class ExemploLancamentoExcecoes {

    // Método que declara lançar uma exceção verificada
    public static void lerArquivo(String nomeArquivo) throws FileNotFoundException {
        if (nomeArquivo == null || nomeArquivo.trim().isEmpty()) {
            throw new IllegalArgumentException("Nome do arquivo não pode ser vazio");
        }
        
        File arquivo = new File(nomeArquivo);
        if (!arquivo.exists()) {
            throw new FileNotFoundException("Arquivo não encontrado: " + nomeArquivo);
        }
        
        System.out.println("Arquivo encontrado: " + nomeArquivo);
    }

    // Método que encapsula exceção
    public static void processarArquivo(String nomeArquivo) {
        try {
            lerArquivo(nomeArquivo);
        } catch (FileNotFoundException e) {
            // Encapsulamento em RuntimeException
            throw new RuntimeException("Erro ao processar arquivo", e);
        }
    }

    // Método com exceção customizada
    public static void autenticar(String usuario, String senha) throws AutenticacaoException {
        if (usuario == null || senha == null) {
            throw new AutenticacaoException("Usuário e senha não podem ser nulos");
        }
        
        if (!usuario.equals("admin") || !senha.equals("1234")) {
            throw new AutenticacaoException("Credenciais inválidas para usuário: " + usuario);
        }
        
        System.out.println("Usuário autenticado: " + usuario);
    }

    // Propagação de exceções
    public static void metodoA() throws FileNotFoundException {
        metodoB();
    }

    public static void metodoB() throws FileNotFoundException {
        metodoC();
    }

    public static void metodoC() throws FileNotFoundException {
        throw new FileNotFoundException("Erro no método C");
    }

    public static void main(String[] args) {
        System.out.println("=== LANÇAMENTO DE EXCEÇÕES ===");

        // Lançando e capturando IllegalArgumentException
        try {
            lerArquivo("");
        } catch (IllegalArgumentException e) {
            System.out.println("Capturada: " + e.getMessage());
        } catch (FileNotFoundException e) {
            System.out.println("Arquivo não encontrado: " + e.getMessage());
        }

        // Encapsulamento de exceção
        try {
            processarArquivo("inexistente.txt");
        } catch (RuntimeException e) {
            System.out.println("RuntimeException: " + e.getMessage());
            System.out.println("Causa original: " + e.getCause().getMessage());
        }

        // Exceção customizada
        try {
            autenticar("admin", "senha_errada");
        } catch (AutenticacaoException e) {
            System.out.println("Falha na autenticação: " + e.getMessage());
            e.registrarLog();
        }

        // Propagação de exceção
        try {
            metodoA();
        } catch (FileNotFoundException e) {
            System.out.println("Exceção propagada: " + e.getMessage());
            e.printStackTrace(); // Mostra a stack trace completa
        }

        // Relançando exceção
        try {
            relancarExcecao();
        } catch (NumberFormatException e) {
            System.out.println("Exceção relançada capturada: " + e.getMessage());
        }

        // Exceções suprimidas (Java 7+)
        demonstrarExcecoesSuprimidas();
    }

    public static void relancarExcecao() {
        try {
            Integer.parseInt("abc");
        } catch (NumberFormatException e) {
            System.out.println("Capturada internamente: " + e.getMessage());
            throw e; // Relançando a exceção
        }
    }

    public static void demonstrarExcecoesSuprimidas() {
        System.out.println("\n=== EXCEÇÕES SUPRIMIDAS ===");

        try (RecursoComExcecao recurso = new RecursoComExcecao()) {
            recurso.operacaoQueFalha();
        } catch (Exception e) {
            System.out.println("Exceção principal: " + e.getMessage());
            
            // Exceções suprimidas
            Throwable[] suprimidas = e.getSuppressed();
            if (suprimidas.length > 0) {
                System.out.println("Exceções suprimidas:");
                for (Throwable suprimida : suprimidas) {
                    System.out.println("  - " + suprimida.getMessage());
                }
            }
        }
    }
}

// Recurso para demonstrar exceções suprimidas
class RecursoComExcecao implements AutoCloseable {
    public void operacaoQueFalha() {
        throw new RuntimeException("Erro durante a operação");
    }

    @Override
    public void close() throws Exception {
        throw new Exception("Erro ao fechar recurso");
    }
}

// Exceção customizada
class AutenticacaoException extends Exception {
    private Date timestamp;

    public AutenticacaoException(String mensagem) {
        super(mensagem);
        this.timestamp = new Date();
    }

    public AutenticacaoException(String mensagem, Throwable causa) {
        super(mensagem, causa);
        this.timestamp = new Date();
    }

    public void registrarLog() {
        System.out.println("LOG [" + timestamp + "]: " + getMessage());
    }

    public Date getTimestamp() {
        return timestamp;
    }
}
```

### **10.2.4 Exceções Customizadas**

**Exemplo 10.4: Criando Hierarquia de Exceções Personalizadas**

```java
import java.util.*;

// Hierarquia de exceções customizadas para um sistema bancário
class BancoException extends Exception {
    public BancoException(String mensagem) {
        super(mensagem);
    }

    public BancoException(String mensagem, Throwable causa) {
        super(mensagem, causa);
    }
}

class SaldoInsuficienteException extends BancoException {
    private double saldoAtual;
    private double valorSaque;

    public SaldoInsuficienteException(double saldoAtual, double valorSaque) {
        super(String.format("Saldo insuficiente. Saldo: R$%.2f, Saque: R$%.2f", 
              saldoAtual, valorSaque));
        this.saldoAtual = saldoAtual;
        this.valorSaque = valorSaque;
    }

    public double getSaldoAtual() { return saldoAtual; }
    public double getValorSaque() { return valorSaque; }
}

class ContaNaoEncontradaException extends BancoException {
    private String numeroConta;

    public ContaNaoEncontradaException(String numeroConta) {
        super("Conta não encontrada: " + numeroConta);
        this.numeroConta = numeroConta;
    }

    public String getNumeroConta() { return numeroConta; }
}

class LimiteExcedidoException extends BancoException {
    private double limite;
    private double valorTransacao;

    public LimiteExcedidoException(double limite, double valorTransacao) {
        super(String.format("Limite excedido. Limite: R$%.2f, Transação: R$%.2f", 
              limite, valorTransacao));
        this.limite = limite;
        this.valorTransacao = valorTransacao;
    }

    public double getLimite() { return limite; }
    public double getValorTransacao() { return valorTransacao; }
}

// Classe que usa as exceções customizadas
class ContaBancaria {
    private String numero;
    private double saldo;
    private double limiteSaque;

    public ContaBancaria(String numero, double saldoInicial, double limiteSaque) {
        this.numero = numero;
        this.saldo = saldoInicial;
        this.limiteSaque = limiteSaque;
    }

    public void sacar(double valor) throws SaldoInsuficienteException, LimiteExcedidoException {
        if (valor > saldo) {
            throw new SaldoInsuficienteException(saldo, valor);
        }
        
        if (valor > limiteSaque) {
            throw new LimiteExcedidoException(limiteSaque, valor);
        }
        
        saldo -= valor;
        System.out.printf("Saque de R$%.2f realizado. Novo saldo: R$%.2f\n", valor, saldo);
    }

    public void depositar(double valor) {
        if (valor <= 0) {
            throw new IllegalArgumentException("Valor de depósito deve ser positivo");
        }
        saldo += valor;
        System.out.printf("Depósito de R$%.2f realizado. Novo saldo: R$%.2f\n", valor, saldo);
    }

    public void transferir(ContaBancaria destino, double valor) 
            throws SaldoInsuficienteException, LimiteExcedidoException {
        System.out.printf("Transferindo R$%.2f para conta %s\n", valor, destino.numero);
        this.sacar(valor); // Pode lançar SaldoInsuficienteException ou LimiteExcedidoException
        destino.depositar(valor);
    }

    // Getters
    public String getNumero() { return numero; }
    public double getSaldo() { return saldo; }
    public double getLimiteSaque() { return limiteSaque; }
}

// Sistema bancário
class SistemaBancario {
    private Map<String, ContaBancaria> contas;

    public SistemaBancario() {
        this.contas = new HashMap<>();
    }

    public void adicionarConta(ContaBancaria conta) {
        contas.put(conta.getNumero(), conta);
    }

    public ContaBancaria buscarConta(String numeroConta) throws ContaNaoEncontradaException {
        ContaBancaria conta = contas.get(numeroConta);
        if (conta == null) {
            throw new ContaNaoEncontradaException(numeroConta);
        }
        return conta;
    }

    public void realizarTransferencia(String contaOrigem, String contaDestino, double valor) 
            throws BancoException {
        try {
            ContaBancaria origem = buscarConta(contaOrigem);
            ContaBancaria destino = buscarConta(contaDestino);
            origem.transferir(destino, valor);
        } catch (ContaNaoEncontradaException e) {
            throw new BancoException("Erro na transferência: " + e.getMessage(), e);
        } catch (SaldoInsuficienteException | LimiteExcedidoException e) {
            throw new BancoException("Erro na transferência: " + e.getMessage(), e);
        }
    }
}

public class ExemploExcecoesCustomizadas {

    public static void main(String[] args) {
        System.out.println("=== EXCEÇÕES CUSTOMIZADAS ===");

        SistemaBancario sistema = new SistemaBancario();
        
        // Criando contas
        ContaBancaria conta1 = new ContaBancaria("123", 1000.00, 500.00);
        ContaBancaria conta2 = new ContaBancaria("456", 500.00, 300.00);
        
        sistema.adicionarConta(conta1);
        sistema.adicionarConta(conta2);

        // Testando operações
        try {
            // Saque válido
            conta1.sacar(200.00);
            
            // Saque com saldo insuficiente
            conta1.sacar(1000.00);
        } catch (SaldoInsuficienteException e) {
            System.out.println("Erro: " + e.getMessage());
        } catch (LimiteExcedidoException e) {
            System.out.println("Erro: " + e.getMessage());
        }

        try {
            // Saque acima do limite
            conta1.sacar(600.00);
        } catch (SaldoInsuficienteException | LimiteExcedidoException e) {
            System.out.println("Erro: " + e.getMessage());
        }

        // Transferência
        try {
            sistema.realizarTransferencia("123", "456", 300.00);
        } catch (BancoException e) {
            System.out.println("Erro na transferência: " + e.getMessage());
            if (e.getCause() != null) {
                System.out.println("Causa: " + e.getCause().getMessage());
            }
        }

        // Transferência para conta inexistente
        try {
            sistema.realizarTransferencia("123", "999", 100.00);
        } catch (BancoException e) {
            System.out.println("Erro na transferência: " + e.getMessage());
            e.printStackTrace(); // Para debug
        }
    }
}
```

### **10.2.5 Try-with-Resources Avançado**

**Exemplo 10.5: Gerenciamento Avançado de Recursos**

```java
import java.io.*;
import java.nio.file.*;
import java.util.*;
import java.util.zip.*;

// Recursos customizados que implementam AutoCloseable
class RecursoCustomizado implements AutoCloseable {
    private String nome;
    private boolean fechado = false;

    public RecursoCustomizado(String nome) {
        this.nome = nome;
        System.out.println("Recurso '" + nome + "' criado");
    }

    public void usar() {
        if (fechado) {
            throw new IllegalStateException("Recurso '" + nome + "' já foi fechado");
        }
        System.out.println("Usando recurso '" + nome + "'");
    }

    @Override
    public void close() {
        if (!fechado) {
            System.out.println("Fechando recurso '" + nome + "'");
            fechado = true;
        }
    }

    public String getNome() { return nome; }
    public boolean isFechado() { return fechado; }
}

class RecursoComExcecao implements AutoCloseable {
    private String nome;

    public RecursoComExcecao(String nome) {
        this.nome = nome;
        System.out.println("Recurso com exceção '" + nome + "' criado");
    }

    public void operacaoQuePodeFalhar() throws IOException {
        throw new IOException("Erro durante operação no recurso " + nome);
    }

    @Override
    public void close() throws Exception {
        System.out.println("Fechando recurso com exceção '" + nome + "'");
        throw new Exception("Erro ao fechar recurso " + nome);
    }
}

public class ExemploTryWithResourcesAvancado {

    public static void main(String[] args) {
        System.out.println("=== TRY-WITH-RESOURCES AVANÇADO ===");

        // Uso básico com recurso customizado
        try (RecursoCustomizado recurso = new RecursoCustomizado("Teste")) {
            recurso.usar();
        } catch (Exception e) {
            System.out.println("Exceção: " + e.getMessage());
        }

        // Múltiplos recursos
        try (RecursoCustomizado recurso1 = new RecursoCustomizado("Primeiro");
             RecursoCustomizado recurso2 = new RecursoCustomizado("Segundo")) {
            
            recurso1.usar();
            recurso2.usar();
        }

        // Recursos são fechados na ordem inversa da declaração
        try (RecursoCustomizado recurso1 = new RecursoCustomizado("A");
             RecursoCustomizado recurso2 = new RecursoCustomizado("B");
             RecursoCustomizado recurso3 = new RecursoCustomizado("C")) {
            
            recurso1.usar();
            recurso2.usar();
            recurso3.usar();
        }

        // Exceção durante o uso e fechamento
        try (RecursoComExcecao recurso = new RecursoComExcecao("Problemático")) {
            recurso.operacaoQuePodeFalhar();
        } catch (Exception e) {
            System.out.println("Exceção capturada: " + e.getMessage());
            // Exceções suprimidas
            if (e.getSuppressed().length > 0) {
                System.out.println("Exceções suprimidas:");
                for (Throwable suprimida : e.getSuppressed()) {
                    System.out.println("  - " + suprimida.getMessage());
                }
            }
        }

        // Trabalhando com arquivos
        processarArquivo("exemplo.txt");
        
        // Processamento de arquivo ZIP
        processarArquivoZip("exemplo.zip");
    }

    public static void processarArquivo(String nomeArquivo) {
        System.out.println("\n=== PROCESSAMENTO DE ARQUIVO ===");

        Path path = Paths.get(nomeArquivo);
        
        // Try-with-resources com BufferedReader
        try (BufferedReader reader = Files.newBufferedReader(path)) {
            String linha;
            while ((linha = reader.readLine()) != null) {
                System.out.println(linha);
            }
        } catch (IOException e) {
            System.out.println("Erro ao processar arquivo: " + e.getMessage());
        }
    }

    public static void processarArquivoZip(String nomeArquivoZip) {
        System.out.println("\n=== PROCESSAMENTO DE ZIP ===");

        try (ZipFile zipFile = new ZipFile(nomeArquivoZip)) {
            Enumeration<? extends ZipEntry> entries = zipFile.entries();
            
            while (entries.hasMoreElements()) {
                ZipEntry entry = entries.nextElement();
                System.out.println("Arquivo no ZIP: " + entry.getName());
                
                // Processar cada entrada
                try (InputStream input = zipFile.getInputStream(entry);
                     BufferedReader reader = new BufferedReader(new InputStreamReader(input))) {
                    
                    String linha;
                    while ((linha = reader.readLine()) != null) {
                        System.out.println("  " + linha);
                    }
                } catch (IOException e) {
                    System.out.println("Erro ao processar entrada: " + e.getMessage());
                }
            }
        } catch (IOException e) {
            System.out.println("Erro ao processar arquivo ZIP: " + e.getMessage());
        }
    }
}
```

### **10.2.6 Assertions**

**Exemplo 10.6: Usando Assertions para Verificação de Invariantes**

```java
public class ExemploAssertions {

    public static void main(String[] args) {
        System.out.println("=== ASSERTIONS ===");

        // As assertions devem ser habilitadas com -ea na JVM
        // java -ea ExemploAssertions

        // Assertion básica
        int idade = 15;
        assert idade >= 0 : "Idade não pode ser negativa: " + idade;
        System.out.println("Idade: " + idade);

        // Assertion em método
        calcularRaizQuadrada(25.0);
        calcularRaizQuadrada(-10.0); // Isso deve lançar AssertionError

        // Assertion para verificar estado do objeto
        Conta conta = new Conta(100.0);
        conta.sacar(50.0);
        conta.sacar(100.0); // Isso deve lançar AssertionError

        // Assertion em construtor
        Pessoa pessoa = new Pessoa("João", 25);
        Pessoa pessoaInvalida = new Pessoa("", -5); // AssertionError

        // Usando assertions para verificar invariantes
        System.out.println("\n=== INVARIANTES ===");
        verificarInvariantes();
    }

    public static double calcularRaizQuadrada(double numero) {
        // Pré-condição
        assert numero >= 0 : "Número não pode ser negativo: " + numero;
        
        double resultado = Math.sqrt(numero);
        
        // Pós-condição
        assert resultado >= 0 : "Resultado não pode ser negativo: " + resultado;
        assert Math.abs(resultado * resultado - numero) < 0.0001 : 
            "Resultado incorreto: " + resultado;
        
        return resultado;
    }

    public static void verificarInvariantes() {
        int[] array = {1, 2, 3, 4, 5};
        
        // Invariante: array não pode ser nulo
        assert array != null : "Array não pode ser nulo";
        
        // Invariante: array deve ter pelo menos um elemento
        assert array.length > 0 : "Array não pode estar vazio";
        
        // Invariante: todos os elementos devem ser positivos
        for (int i = 0; i < array.length; i++) {
            assert array[i] > 0 : "Elemento na posição " + i + " não é positivo: " + array[i];
        }
        
        System.out.println("Todos os invariantes foram verificados");
    }
}

class Conta {
    private double saldo;

    public Conta(double saldoInicial) {
        // Invariante: saldo não pode ser negativo
        assert saldoInicial >= 0 : "Saldo inicial não pode ser negativo: " + saldoInicial;
        this.saldo = saldoInicial;
    }

    public void sacar(double valor) {
        // Pré-condição
        assert valor > 0 : "Valor do saque deve ser positivo: " + valor;
        
        double saldoAnterior = saldo;
        saldo -= valor;
        
        // Pós-condição
        assert saldo >= 0 : "Saldo não pode ficar negativo: " + saldo;
        assert saldo == saldoAnterior - valor : "Cálculo do saldo incorreto";
        
        System.out.println("Saque de " + valor + " realizado. Novo saldo: " + saldo);
    }

    public void depositar(double valor) {
        assert valor > 0 : "Valor do depósito deve ser positivo: " + valor;
        
        double saldoAnterior = saldo;
        saldo += valor;
        
        assert saldo == saldoAnterior + valor : "Cálculo do saldo incorreto";
        System.out.println("Depósito de " + valor + " realizado. Novo saldo: " + saldo);
    }

    public double getSaldo() {
        return saldo;
    }
}

class Pessoa {
    private String nome;
    private int idade;

    public Pessoa(String nome, int idade) {
        // Verificações de invariantes com assertions
        assert nome != null && !nome.trim().isEmpty() : "Nome não pode ser nulo ou vazio";
        assert idade >= 0 && idade <= 150 : "Idade inválida: " + idade;
        
        this.nome = nome;
        this.idade = idade;
        System.out.println("Pessoa criada: " + nome + ", " + idade + " anos");
    }

    public String getNome() { return nome; }
    public int getIdade() { return idade; }
}
```

## **10.3 Exercícios Práticos**

### **Exercício 10.1: Validador de Dados com Exceções Customizadas**

```java
import java.util.*;
import java.util.regex.*;

// Exceções customizadas para validação
class ValidacaoException extends Exception {
    public ValidacaoException(String mensagem) {
        super(mensagem);
    }
}

class EmailInvalidoException extends ValidacaoException {
    public EmailInvalidoException(String email) {
        super("Email inválido: " + email);
    }
}

class SenhaFracaException extends ValidacaoException {
    public SenhaFracaException() {
        super("Senha não atende aos requisitos de segurança");
    }
}

class CPFInvalidoException extends ValidacaoException {
    public CPFInvalidoException(String cpf) {
        super("CPF inválido: " + cpf);
    }
}

class IdadeInvalidaException extends ValidacaoException {
    public IdadeInvalidaException(int idade) {
        super("Idade inválida: " + idade);
    }
}

// Validador de dados
class Validador {
    private static final Pattern EMAIL_PATTERN = 
        Pattern.compile("^[A-Za-z0-9+_.-]+@[A-Za-z0-9.-]+$");
    
    private static final Pattern SENHA_PATTERN = 
        Pattern.compile("^(?=.*[0-9])(?=.*[a-z])(?=.*[A-Z])(?=.*[@#$%^&+=])(?=\\S+$).{8,}$");

    public static void validarEmail(String email) throws EmailInvalidoException {
        if (email == null || !EMAIL_PATTERN.matcher(email).matches()) {
            throw new EmailInvalidoException(email);
        }
    }

    public static void validarSenha(String senha) throws SenhaFracaException {
        if (senha == null || !SENHA_PATTERN.matcher(senha).matches()) {
            throw new SenhaFracaException();
        }
    }

    public static void validarCPF(String cpf) throws CPFInvalidoException {
        if (cpf == null || !validarCPFNumerico(cpf)) {
            throw new CPFInvalidoException(cpf);
        }
    }

    public static void validarIdade(int idade) throws IdadeInvalidaException {
        if (idade < 0 || idade > 150) {
            throw new IdadeInvalidaException(idade);
        }
    }

    private static boolean validarCPFNumerico(String cpf) {
        // Remover caracteres não numéricos
        cpf = cpf.replaceAll("\\D", "");
        
        // Verificar se tem 11 dígitos
        if (cpf.length() != 11) {
            return false;
        }
        
        // Verificar se todos os dígitos são iguais
        if (cpf.matches("(\\d)\\1{10}")) {
            return false;
        }
        
        // Algoritmo de validação do CPF
        try {
            int[] digitos = new int[11];
            for (int i = 0; i < 11; i++) {
                digitos[i] = Integer.parseInt(cpf.substring(i, i + 1));
            }
            
            // Calcular primeiro dígito verificador
            int soma = 0;
            for (int i = 0; i < 9; i++) {
                soma += digitos[i] * (10 - i);
            }
            int resto = soma % 11;
            int digito1 = (resto < 2) ? 0 : 11 - resto;
            
            // Calcular segundo dígito verificador
            soma = 0;
            for (int i = 0; i < 10; i++) {
                soma += digitos[i] * (11 - i);
            }
            resto = soma % 11;
            int digito2 = (resto < 2) ? 0 : 11 - resto;
            
            // Verificar dígitos
            return (digitos[9] == digito1 && digitos[10] == digito2);
        } catch (NumberFormatException e) {
            return false;
        }
    }
}

// Sistema de cadastro de usuários
class SistemaCadastro {
    private List<Usuario> usuarios;

    public SistemaCadastro() {
        this.usuarios = new ArrayList<>();
    }

    public void cadastrarUsuario(String nome, String email, String senha, String cpf, int idade) 
            throws ValidacaoException {
        // Validar todos os dados
        Validador.validarEmail(email);
        Validador.validarSenha(senha);
        Validador.validarCPF(cpf);
        Validador.validarIdade(idade);

        // Verificar se email já existe
        for (Usuario usuario : usuarios) {
            if (usuario.getEmail().equals(email)) {
                throw new ValidacaoException("Email já cadastrado: " + email);
            }
        }

        // Criar e adicionar usuário
        Usuario novoUsuario = new Usuario(nome, email, senha, cpf, idade);
        usuarios.add(novoUsuario);
        System.out.println("Usuário cadastrado com sucesso: " + nome);
    }

    public void listarUsuarios() {
        System.out.println("\n=== USUÁRIOS CADASTRADOS ===");
        for (Usuario usuario : usuarios) {
            System.out.println(usuario);
        }
    }
}

class Usuario {
    private String nome;
    private String email;
    private String senha;
    private String cpf;
    private int idade;

    public Usuario(String nome, String email, String senha, String cpf, int idade) {
        this.nome = nome;
        this.email = email;
        this.senha = senha;
        this.cpf = cpf;
        this.idade = idade;
    }

    // Getters
    public String getNome() { return nome; }
    public String getEmail() { return email; }
    public String getSenha() { return senha; }
    public String getCpf() { return cpf; }
    public int getIdade() { return idade; }

    @Override
    public String toString() {
        return String.format("Usuario{nome='%s', email='%s', cpf='%s', idade=%d}",
                nome, email, cpf, idade);
    }
}

public class ExercicioValidador {

    public static void main(String[] args) {
        SistemaCadastro sistema = new SistemaCadastro();

        // Testes de cadastro
        try {
            // Cadastro válido
            sistema.cadastrarUsuario(
                "João Silva", 
                "joao.silva@email.com", 
                "Senha@123", 
                "123.456.789-09", 
                30
            );

            // Email inválido
            sistema.cadastrarUsuario(
                "Maria Santos", 
                "email-invalido", 
                "Senha@123", 
                "987.654.321-00", 
                25
            );
        } catch (ValidacaoException e) {
            System.out.println("Erro no cadastro: " + e.getMessage());
        }

        try {
            // Senha fraca
            sistema.cadastrarUsuario(
                "Carlos Oliveira", 
                "carlos@email.com", 
                "123", 
                "111.444.777-35", 
                35
            );
        } catch (ValidacaoException e) {
            System.out.println("Erro no cadastro: " + e.getMessage());
        }

        try {
            // CPF inválido
            sistema.cadastrarUsuario(
                "Ana Costa", 
                "ana@email.com", 
                "Senha@123", 
                "000.000.000-00", 
                28
            );
        } catch (ValidacaoException e) {
            System.out.println("Erro no cadastro: " + e.getMessage());
        }

        try {
            // Idade inválida
            sistema.cadastrarUsuario(
                "Pedro Alves", 
                "pedro@email.com", 
                "Senha@123", 
                "222.333.444-55", 
                -5
            );
        } catch (ValidacaoException e) {
            System.out.println("Erro no cadastro: " + e.getMessage());
        }

        // Listar usuários cadastrados
        sistema.listarUsuarios();
    }
}
```

### **Exercício 10.2: Sistema de Log com Try-with-Resources**

```java
import java.io.*;
import java.nio.file.*;
import java.time.*;
import java.time.format.*;
import java.util.*;
import java.util.concurrent.*;

// Logger customizado com try-with-resources
class FileLogger implements AutoCloseable {
    private BufferedWriter writer;
    private String logFile;
    private boolean isClosed = false;

    public FileLogger(String logFile) throws IOException {
        this.logFile = logFile;
        this.writer = Files.newBufferedWriter(Paths.get(logFile), 
                       StandardOpenOption.CREATE, StandardOpenOption.APPEND);
        log("INFO", "Logger iniciado");
    }

    public void log(String level, String message) {
        if (isClosed) {
            throw new IllegalStateException("Logger está fechado");
        }

        try {
            String timestamp = LocalDateTime.now()
                    .format(DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss"));
            String logEntry = String.format("[%s] %s: %s%n", timestamp, level, message);
            writer.write(logEntry);
            writer.flush(); // Garante que seja escrito imediatamente
        } catch (IOException e) {
            System.err.println("Erro ao escrever no log: " + e.getMessage());
        }
    }

    public void info(String message) {
        log("INFO", message);
    }

    public void warn(String message) {
        log("WARN", message);
    }

    public void error(String message) {
        log("ERROR", message);
    }

    public void error(String message, Throwable throwable) {
        log("ERROR", message + " - " + throwable.getMessage());
        // Poderia também escrever o stack trace
    }

    @Override
    public void close() throws Exception {
        if (!isClosed) {
            log("INFO", "Logger finalizado");
            writer.close();
            isClosed = true;
        }
    }
}

// Serviço que usa o logger
class ServicoProcessamento {
    private FileLogger logger;

    public ServicoProcessamento(FileLogger logger) {
        this.logger = logger;
    }

    public void processarArquivo(String arquivoEntrada, String arquivoSaida) {
        logger.info("Iniciando processamento do arquivo: " + arquivoEntrada);

        try (BufferedReader reader = Files.newBufferedReader(Paths.get(arquivoEntrada));
             BufferedWriter writer = Files.newBufferedWriter(Paths.get(arquivoSaida))) {

            String linha;
            int contador = 0;
            while ((linha = reader.readLine()) != null) {
                // Simular processamento
                String linhaProcessada = linha.toUpperCase();
                writer.write(linhaProcessada);
                writer.newLine();
                contador++;

                // Simular erro a cada 100 linhas para teste
                if (contador % 100 == 0) {
                    if (Math.random() < 0.1) { // 10% de chance de erro
                        throw new IOException("Erro simulado na linha " + contador);
                    }
                }
            }

            logger.info("Processamento concluído. " + contador + " linhas processadas");

        } catch (IOException e) {
            logger.error("Erro durante o processamento do arquivo", e);
            throw new RuntimeException("Falha no processamento", e);
        }
    }

    public void processarLote(List<String> arquivos) {
        logger.info("Iniciando processamento em lote de " + arquivos.size() + " arquivos");

        for (String arquivo : arquivos) {
            String saida = arquivo.replace(".txt", "_processado.txt");
            try {
                processarArquivo(arquivo, saida);
            } catch (Exception e) {
                logger.warn("Falha ao processar arquivo: " + arquivo + " - " + e.getMessage());
                // Continua com o próximo arquivo
            }
        }

        logger.info("Processamento em lote concluído");
    }
}

// Gerenciador de recursos com pool
class LoggerPool {
    private BlockingQueue<FileLogger> pool;
    private String logFile;
    private int maxSize;

    public LoggerPool(String logFile, int poolSize) {
        this.logFile = logFile;
        this.maxSize = poolSize;
        this.pool = new ArrayBlockingQueue<>(poolSize);

        // Inicializar pool com loggers
        for (int i = 0; i < poolSize; i++) {
            try {
                pool.offer(new FileLogger(logFile + "." + i));
            } catch (IOException e) {
                System.err.println("Erro ao criar logger: " + e.getMessage());
            }
        }
    }

    public FileLogger getLogger() throws InterruptedException {
        FileLogger logger = pool.take();
        // Se o logger estiver fechado, criar um novo
        if (isClosed(logger)) {
            try {
                logger = new FileLogger(logFile + "." + System.currentTimeMillis());
            } catch (IOException e) {
                // Retornar null ou lançar exceção
                System.err.println("Erro ao criar novo logger: " + e.getMessage());
                return null;
            }
        }
        return logger;
    }

    public void returnLogger(FileLogger logger) {
        if (logger != null && !isClosed(logger)) {
            pool.offer(logger);
        }
    }

    public void closeAll() {
        for (FileLogger logger : pool) {
            try {
                if (!isClosed(logger)) {
                    logger.close();
                }
            } catch (Exception e) {
                System.err.println("Erro ao fechar logger: " + e.getMessage());
            }
        }
    }

    private boolean isClosed(FileLogger logger) {
        // Verificação simplificada - na implementação real precisaria de um método
        try {
            logger.info("Teste"); // Tenta usar o logger
            return false;
        } catch (IllegalStateException e) {
            return true;
        }
    }
}

public class ExercicioSistemaLog {

    public static void main(String[] args) {
        System.out.println("=== SISTEMA DE LOG COM TRY-WITH-RESOURCES ===");

        // Exemplo com try-with-resources simples
        try (FileLogger logger = new FileLogger("aplicacao.log")) {
            logger.info("Aplicação iniciada");
            
            // Simular processamento
            ServicoProcessamento servico = new ServicoProcessamento(logger);
            
            // Criar arquivo de teste
            criarArquivoTeste("dados_entrada.txt");
            
            // Processar arquivo
            servico.processarArquivo("dados_entrada.txt", "dados_saida.txt");
            
            logger.info("Aplicação finalizada com sucesso");
            
        } catch (Exception e) {
            System.err.println("Erro na aplicação: " + e.getMessage());
        }

        // Exemplo com pool de loggers
        testarLoggerPool();
    }

    public static void criarArquivoTeste(String nomeArquivo) {
        try (BufferedWriter writer = Files.newBufferedWriter(Paths.get(nomeArquivo))) {
            for (int i = 1; i <= 1000; i++) {
                writer.write("Linha " + i + " - Dados de exemplo para processamento");
                writer.newLine();
            }
        } catch (IOException e) {
            System.err.println("Erro ao criar arquivo de teste: " + e.getMessage());
        }
    }

    public static void testarLoggerPool() {
        System.out.println("\n=== TESTE COM POOL DE LOGGERS ===");

        LoggerPool pool = new LoggerPool("pool", 3);

        ExecutorService executor = Executors.newFixedThreadPool(5);

        for (int i = 0; i < 10; i++) {
            final int taskId = i;
            executor.submit(() -> {
                try {
                    FileLogger logger = pool.getLogger();
                    if (logger != null) {
                        try {
                            logger.info("Task " + taskId + " iniciada pela thread " + 
                                      Thread.currentThread().getName());
                            
                            // Simular trabalho
                            Thread.sleep(1000);
                            
                            logger.info("Task " + taskId + " concluída");
                        } finally {
                            pool.returnLogger(logger);
                        }
                    }
                } catch (InterruptedException e) {
                    Thread.currentThread().interrupt();
                }
            });
        }

        executor.shutdown();
        try {
            executor.awaitTermination(10, TimeUnit.SECONDS);
            pool.closeAll();
        } catch (InterruptedException e) {
            Thread.currentThread().interrupt();
        }
    }
}
```

## **10.4 Caso Prático: Sistema de Transações Financeiras com Rollback**

```java
import java.io.*;
import java.nio.file.*;
import java.util.*;
import java.util.concurrent.atomic.*;

// Exceções para transações
class TransacaoException extends Exception {
    public TransacaoException(String mensagem) {
        super(mensagem);
    }

    public TransacaoException(String mensagem, Throwable causa) {
        super(mensagem, causa);
    }
}

class SaldoInsuficienteException extends TransacaoException {
    public SaldoInsuficienteException(double saldo, double valor) {
        super(String.format("Saldo insuficiente. Saldo: %.2f, Valor: %.2f", saldo, valor));
    }
}

class ContaBloqueadaException extends TransacaoException {
    public ContaBloqueadaException(String numeroConta) {
        super("Conta bloqueada: " + numeroConta);
    }
}

// Interface para operações de transação
interface Operacao {
    void executar() throws TransacaoException;
    void reverter() throws TransacaoException;
}

// Implementações concretas de operações
class OperacaoSaque implements Operacao {
    private Conta conta;
    private double valor;

    public OperacaoSaque(Conta conta, double valor) {
        this.conta = conta;
        this.valor = valor;
    }

    @Override
    public void executar() throws TransacaoException {
        conta.sacar(valor);
    }

    @Override
    public void reverter() throws TransacaoException {
        conta.depositar(valor);
    }
}

class OperacaoDeposito implements Operacao {
    private Conta conta;
    private double valor;

    public OperacaoDeposito(Conta conta, double valor) {
        this.conta = conta;
        this.valor = valor;
    }

    @Override
    public void executar() throws TransacaoException {
        conta.depositar(valor);
    }

    @Override
    public void reverter() throws TransacaoException {
        conta.sacar(valor);
    }
}

class OperacaoTransferencia implements Operacao {
    private Conta origem;
    private Conta destino;
    private double valor;

    public OperacaoTransferencia(Conta origem, Conta destino, double valor) {
        this.origem = origem;
        this.destino = destino;
        this.valor = valor;
    }

    @Override
    public void executar() throws TransacaoException {
        origem.sacar(valor);
        destino.depositar(valor);
    }

    @Override
    public void reverter() throws TransacaoException {
        destino.sacar(valor);
        origem.depositar(valor);
    }
}

// Gerenciador de transações
class Transacao {
    private List<Operacao> operacoes;
    private boolean concluida;

    public Transacao() {
        this.operacoes = new ArrayList<>();
        this.concluida = false;
    }

    public void adicionarOperacao(Operacao operacao) {
        if (concluida) {
            throw new IllegalStateException("Transação já foi concluída");
        }
        operacoes.add(operacao);
    }

    public void executar() throws TransacaoException {
        if (concluida) {
            throw new IllegalStateException("Transação já foi concluída");
        }

        List<Operacao> executadasComSucesso = new ArrayList<>();

        try {
            for (Operacao operacao : operacoes) {
                operacao.executar();
                executadasComSucesso.add(operacao);
            }
            concluida = true;
        } catch (TransacaoException e) {
            // Rollback das operações já executadas
            for (int i = executadasComSucesso.size() - 1; i >= 0; i--) {
                try {
                    executadasComSucesso.get(i).reverter();
                } catch (TransacaoException reverterEx) {
                    // Log do erro no rollback, mas não interrompe o rollback
                    System.err.println("Erro ao reverter operação: " + reverterEx.getMessage());
                }
            }
            throw new TransacaoException("Falha na transação. Rollback executado.", e);
        }
    }

    public boolean isConcluida() {
        return concluida;
    }
}

// Conta bancária com suporte a transações
class Conta {
    private String numero;
    private double saldo;
    private boolean bloqueada;
    private AtomicInteger sequencialTransacao = new AtomicInteger(0);

    public Conta(String numero, double saldoInicial) {
        this.numero = numero;
        this.saldo = saldoInicial;
        this.bloqueada = false;
    }

    public void sacar(double valor) throws TransacaoException {
        if (bloqueada) {
            throw new ContaBloqueadaException(numero);
        }
        if (valor > saldo) {
            throw new SaldoInsuficienteException(saldo, valor);
        }
        if (valor <= 0) {
            throw new TransacaoException("Valor de saque deve ser positivo: " + valor);
        }

        saldo -= valor;
        System.out.printf("Saque: R$%.2f da conta %s. Novo saldo: R$%.2f%n", 
                         valor, numero, saldo);
    }

    public void depositar(double valor) throws TransacaoException {
        if (bloqueada) {
            throw new ContaBloqueadaException(numero);
        }
        if (valor <= 0) {
            throw new TransacaoException("Valor de depósito deve ser positivo: " + valor);
        }

        saldo += valor;
        System.out.printf("Depósito: R$%.2f na conta %s. Novo saldo: R$%.2f%n", 
                         valor, numero, saldo);
    }

    public void bloquear() {
        this.bloqueada = true;
        System.out.println("Conta " + numero + " bloqueada");
    }

    public void desbloquear() {
        this.bloqueada = false;
        System.out.println("Conta " + numero + " desbloqueada");
    }

    // Getters
    public String getNumero() { return numero; }
    public double getSaldo() { return saldo; }
    public boolean isBloqueada() { return bloqueada; }
}

// Sistema bancário com suporte a transações
class SistemaBancarioTransacional {
    private Map<String, Conta> contas;

    public SistemaBancarioTransacional() {
        this.contas = new HashMap<>();
    }

    public void adicionarConta(Conta conta) {
        contas.put(conta.getNumero(), conta);
    }

    public Conta getConta(String numero) {
        return contas.get(numero);
    }

    public void transferir(String contaOrigem, String contaDestino, double valor) 
            throws TransacaoException {
        Conta origem = contas.get(contaOrigem);
        Conta destino = contas.get(contaDestino);

        if (origem == null) {
            throw new TransacaoException("Conta origem não encontrada: " + contaOrigem);
        }
        if (destino == null) {
            throw new TransacaoException("Conta destino não encontrada: " + contaDestino);
        }

        Transacao transacao = new Transacao();
        transacao.adicionarOperacao(new OperacaoSaque(origem, valor));
        transacao.adicionarOperacao(new OperacaoDeposito(destino, valor));

        transacao.executar();
        System.out.println("Transferência concluída com sucesso");
    }

    public void processarLoteTransacoes(List<Transacao> transacoes) {
        int sucessos = 0;
        int falhas = 0;

        for (Transacao transacao : transacoes) {
            try {
                transacao.executar();
                sucessos++;
            } catch (TransacaoException e) {
                falhas++;
                System.err.println("Transação falhou: " + e.getMessage());
            }
        }

        System.out.printf("Lote processado: %d sucessos, %d falhas%n", sucessos, falhas);
    }
}

public class CasoPraticoTransacoes {

    public static void main(String[] args) {
        System.out.println("=== SISTEMA DE TRANSAÇÕES FINANCEIRAS ===");

        SistemaBancarioTransacional sistema = new SistemaBancarioTransacional();

        // Criar contas
        Conta conta1 = new Conta("001", 1000.00);
        Conta conta2 = new Conta("002", 500.00);
        Conta conta3 = new Conta("003", 200.00);

        sistema.adicionarConta(conta1);
        sistema.adicionarConta(conta2);
        sistema.adicionarConta(conta3);

        // Teste de transferência bem-sucedida
        try {
            sistema.transferir("001", "002", 200.00);
        } catch (TransacaoException e) {
            System.out.println("Transferência falhou: " + e.getMessage());
        }

        // Teste de transferência com saldo insuficiente
        try {
            sistema.transferir("003", "001", 500.00);
        } catch (TransacaoException e) {
            System.out.println("Transferência falhou: " + e.getMessage());
        }

        // Teste com conta bloqueada
        conta1.bloquear();
        try {
            sistema.transferir("001", "002", 100.00);
        } catch (TransacaoException e) {
            System.out.println("Transferência falhou: " + e.getMessage());
        }
        conta1.desbloquear();

        // Transação complexa com múltiplas operações
        try {
            Transacao transacaoComplexa = new Transacao();
            transacaoComplexa.adicionarOperacao(new OperacaoSaque(conta1, 100.00));
            transacaoComplexa.adicionarOperacao(new OperacaoDeposito(conta2, 50.00));
            transacaoComplexa.adicionarOperacao(new OperacaoDeposito(conta3, 50.00));

            transacaoComplexa.executar();
            System.out.println("Transação complexa executada com sucesso");
        } catch (TransacaoException e) {
            System.out.println("Transação complexa falhou: " + e.getMessage());
        }

        // Processamento em lote
        List<Transacao> lote = new ArrayList<>();
        
        Transacao t1 = new Transacao();
        t1.adicionarOperacao(new OperacaoTransferencia(conta1, conta2, 50.00));
        lote.add(t1);

        Transacao t2 = new Transacao();
        t2.adicionarOperacao(new OperacaoTransferencia(conta2, conta3, 1000.00)); // Deve falhar
        lote.add(t2);

        Transacao t3 = new Transacao();
        t3.adicionarOperacao(new OperacaoTransferencia(conta3, conta1, 30.00));
        lote.add(t3);

        sistema.processarLoteTransacoes(lote);

        // Verificar saldos finais
        System.out.println("\n=== SALDOS FINAIS ===");
        System.out.printf("Conta %s: R$%.2f%n", conta1.getNumero(), conta1.getSaldo());
        System.out.printf("Conta %s: R$%.2f%n", conta2.getNumero(), conta2.getSaldo());
        System.out.printf("Conta %s: R$%.2f%n", conta3.getNumero(), conta3.getSaldo());
    }
}
```

## **10.5 Questionário de Revisão**

**Questão 1:** Qual a diferença entre exceções verificadas e não verificadas?
- A) Verificadas: herdam de Exception, devem ser tratadas. Não verificadas: herdam de RuntimeException
- B) Verificadas: erros de programação. Não verificadas: erros de sistema
- C) Verificadas: podem ser ignoradas. Não verificadas: devem ser tratadas

**Questão 2:** O que é o bloco `finally` usado para?
- A) Executar código independentemente de exceções ocorrerem ou não
- B) Capturar exceções específicas
- C) Lançar exceções personalizadas

**Questão 3:** Qual a vantagem do try-with-resources?
- A) Fechamento automático de recursos que implementam AutoCloseable
- B) Melhor performance no tratamento de exceções
- C) Substitui completamente o bloco catch

**Questão 4:** Quando usar assertions em Java?
- A) Para verificar invariantes durante o desenvolvimento
- B) Para tratamento de erros em produção
- C) Para validar entrada de usuário

**Questão 5:** O que é exceção suprimida no try-with-resources?
- A) Exceção lançada no close() quando já há uma exceção no try
- B) Exceção ignorada pelo compilador
- C) Exceção capturada automaticamente

## **10.6 Laboratório Prático**

**Projeto: Sistema de Gerenciamento de Arquivos com Tratamento de Erros**

```java
// Implemente um sistema que:
// 1. Copie arquivos com verificação de espaço em disco
// 2. Valide permissões de leitura/escrita
// 3. Implemente rollback em caso de erro
// 4. Log todas as operações e erros
// 5. Use try-with-resources para gerenciar recursos

// Use: exceções customizadas, try-with-resources, logging, assertions
```

## **10.7 Material de Apoio**

**Hierarquia de Exceções:**
```
Throwable
├── Error
│   ├── OutOfMemoryError
│   ├── StackOverflowError
│   └── ...
└── Exception
    ├── RuntimeException (Unchecked)
    │   ├── NullPointerException
    │   ├── IllegalArgumentException
    │   ├── IndexOutOfBoundsException
    │   └── ...
    └── Checked Exceptions
        ├── IOException
        ├── SQLException
        ├── FileNotFoundException
        └── ...
```

**Melhores Práticas:**
- Use exceções apenas para situações excepcionais
- Prefira exceções unchecked para erros de programação
- Documente as exceções que seu método lança
- Mantenha as mensagens de erro claras e informativas
- Use try-with-resources para recursos que precisam ser fechados
- Não ignore exceções vazias no catch

**Padrões Comuns:**
- Exception Chaining: encapsule exceções originais
- Custom Exceptions: para erros específicos do domínio
- Resource Management: use try-with-resources
- Assertions: para verificação de invariantes

**Dicas de Performance:**
- Construa a stack trace apenas quando necessário
- Evite exceções em loops de performance crítica
- Use exceptions para casos excepcionais, não para controle de fluxo

---

**Próximo Módulo: Programação Concorrente em Java**

Preparado para explorar threads, executors e programação paralela?

---

# **Módulo 11: Programação Concorrente em Java**

## **11.1 Objetivos do Módulo**

- Compreender os fundamentos de threads e concorrência
- Dominar a criação e gerenciamento de threads
- Aprender a usar o Framework Executor para gerenciamento de threads
- Conhecer as coleções thread-safe do Java
- Dominar os mecanismos de sincronização e locks
- Aprender sobre programação assíncrona com CompletableFuture
- Entender padrões comuns de concorrência

## **11.2 Conteúdo Programático**

### **11.2.1 Fundamentos de Threads**

**Exemplo 11.1: Criando e Gerenciando Threads**

```java
public class ExemploThreads {

    public static void main(String[] args) {
        System.out.println("=== FUNDAMENTOS DE THREADS ===");
        
        // Thread atual (main)
        Thread threadPrincipal = Thread.currentThread();
        System.out.println("Thread principal: " + threadPrincipal.getName());
        System.out.println("ID: " + threadPrincipal.getId());
        System.out.println("Prioridade: " + threadPrincipal.getPriority());
        System.out.println("Estado: " + threadPrincipal.getState());
        System.out.println("É daemon? " + threadPrincipal.isDaemon());
        
        // Criando threads
        criarThreads();
        gerenciarThreads();
        estadosThread();
    }
    
    public static void criarThreads() {
        System.out.println("\n=== CRIANDO THREADS ===");
        
        // Método 1: Estendendo Thread
        class MinhaThread extends Thread {
            private String nome;
            
            public MinhaThread(String nome) {
                this.nome = nome;
            }
            
            @Override
            public void run() {
                System.out.println(nome + " está executando na thread: " + 
                                 Thread.currentThread().getName());
                try {
                    Thread.sleep(2000); // Simula trabalho
                } catch (InterruptedException e) {
                    System.out.println(nome + " foi interrompida");
                }
                System.out.println(nome + " terminou");
            }
        }
        
        // Método 2: Implementando Runnable
        class MeuRunnable implements Runnable {
            private String nome;
            
            public MeuRunnable(String nome) {
                this.nome = nome;
            }
            
            @Override
            public void run() {
                System.out.println(nome + " está executando na thread: " + 
                                 Thread.currentThread().getName());
                try {
                    Thread.sleep(1500);
                } catch (InterruptedException e) {
                    System.out.println(nome + " foi interrompido");
                }
                System.out.println(nome + " terminou");
            }
        }
        
        // Criando e iniciando threads
        Thread t1 = new MinhaThread("Thread-1");
        Thread t2 = new Thread(new MeuRunnable("Runnable-1"));
        Thread t3 = new Thread(() -> {
            System.out.println("Lambda Runnable executando na thread: " + 
                             Thread.currentThread().getName());
            try {
                Thread.sleep(1000);
            } catch (InterruptedException e) {
                System.out.println("Lambda interrompida");
            }
            System.out.println("Lambda terminou");
        }, "Thread-Lambda");
        
        t1.start();
        t2.start();
        t3.start();
        
        // Aguardando threads terminarem
        try {
            t1.join();
            t2.join();
            t3.join();
        } catch (InterruptedException e) {
            e.printStackTrace();
        }
        
        System.out.println("Todas as threads terminaram");
    }
    
    public static void gerenciarThreads() {
        System.out.println("\n=== GERENCIANDO THREADS ===");
        
        Thread t1 = new Thread(() -> {
            for (int i = 1; i <= 5; i++) {
                System.out.println(Thread.currentThread().getName() + " - Contador: " + i);
                try {
                    Thread.sleep(500);
                } catch (InterruptedException e) {
                    System.out.println(Thread.currentThread().getName() + " interrompida");
                    return; // Termina a thread se interrompida
                }
            }
        }, "Thread-Gerenciada");
        
        // Configurações
        t1.setPriority(Thread.MAX_PRIORITY);
        t1.setDaemon(false); // Thread de usuário (não daemon)
        
        System.out.println("Antes de iniciar:");
        System.out.println("Nome: " + t1.getName());
        System.out.println("Prioridade: " + t1.getPriority());
        System.out.println("É daemon? " + t1.isDaemon());
        System.out.println("Estado: " + t1.getState());
        System.out.println("Está viva? " + t1.isAlive());
        
        t1.start();
        
        System.out.println("\nDepois de iniciar:");
        System.out.println("Estado: " + t1.getState());
        System.out.println("Está viva? " + t1.isAlive());
        
        // Interrompendo a thread após 1 segundo
        try {
            Thread.sleep(1000);
            t1.interrupt(); // Envia sinal de interrupção
        } catch (InterruptedException e) {
            e.printStackTrace();
        }
        
        // Aguardando thread terminar
        try {
            t1.join(2000); // Timeout de 2 segundos
            if (t1.isAlive()) {
                System.out.println("Thread ainda está executando após timeout");
            } else {
                System.out.println("Thread terminou normalmente");
            }
        } catch (InterruptedException e) {
            e.printStackTrace();
        }
    }
    
    public static void estadosThread() {
        System.out.println("\n=== ESTADOS DE THREAD ===");
        
        Thread t1 = new Thread(() -> {
            System.out.println("Thread iniciada, estado: " + Thread.currentThread().getState());
            
            try {
                Thread.sleep(1000); // Vai para TIMED_WAITING
                synchronized (EstadosThreads.class) {
                    EstadosThreads.class.wait(); // Vai para WAITING
                }
            } catch (InterruptedException e) {
                System.out.println("Thread interrompida");
            }
            
            System.out.println("Thread terminando, estado: " + Thread.currentThread().getState());
        }, "Thread-Estados");
        
        // Monitorando estados
        new Thread(() -> {
            Thread.State estadoAnterior = null;
            while (t1.isAlive()) {
                Thread.State estadoAtual = t1.getState();
                if (estadoAtual != estadoAnterior) {
                    System.out.println("Estado da thread: " + estadoAtual);
                    estadoAnterior = estadoAtual;
                }
                try {
                    Thread.sleep(100);
                } catch (InterruptedException e) {
                    break;
                }
            }
        }, "Monitor").start();
        
        t1.start();
        
        try {
            Thread.sleep(1500);
            synchronized (EstadosThreads.class) {
                EstadosThreads.class.notify(); // Tira da WAITING
            }
            Thread.sleep(500);
            t1.interrupt();
            t1.join();
        } catch (InterruptedException e) {
            e.printStackTrace();
        }
    }
}

class EstadosThreads {
    // Classe auxiliar para demonstração
}
```

### **11.2.2 Sincronização e Locks**

**Exemplo 11.2: Controle de Acesso com Sincronização**

```java
import java.util.concurrent.locks.*;

public class ExemploSincronizacao {

    public static void main(String[] args) {
        System.out.println("=== SINCRONIZAÇÃO E LOCKS ===");
        
        // Problema de condição de corrida
        demonstrarCondicaoCorrida();
        
        // Solução com synchronized
        demonstrarSynchronized();
        
        // Locks explícitos
        demonstrarLocks();
        
        // Deadlock
        demonstrarDeadlock();
        
        // Wait e Notify
        demonstrarWaitNotify();
    }
    
    public static void demonstrarCondicaoCorrida() {
        System.out.println("\n=== CONDIÇÃO DE CORRIDA ===");
        
        class Contador {
            private int valor = 0;
            
            public void incrementar() {
                valor++; // Não é atômico!
            }
            
            public int getValor() {
                return valor;
            }
        }
        
        Contador contador = new Contador();
        
        // Criando múltiplas threads que incrementam o contador
        Thread[] threads = new Thread[10];
        for (int i = 0; i < threads.length; i++) {
            threads[i] = new Thread(() -> {
                for (int j = 0; j < 1000; j++) {
                    contador.incrementar();
                }
            });
        }
        
        // Iniciando todas as threads
        for (Thread t : threads) {
            t.start();
        }
        
        // Aguardando todas terminarem
        for (Thread t : threads) {
            try {
                t.join();
            } catch (InterruptedException e) {
                e.printStackTrace();
            }
        }
        
        System.out.println("Valor esperado: 10000");
        System.out.println("Valor real: " + contador.getValor());
        System.out.println("Problema de condição de corrida evidente!");
    }
    
    public static void demonstrarSynchronized() {
        System.out.println("\n=== SINCHRONIZED ===");
        
        class ContadorSincronizado {
            private int valor = 0;
            
            // Método sincronizado
            public synchronized void incrementar() {
                valor++;
            }
            
            // Bloco sincronizado
            public void incrementarComBloco() {
                synchronized (this) {
                    valor++;
                }
            }
            
            public synchronized int getValor() {
                return valor;
            }
        }
        
        ContadorSincronizado contador = new ContadorSincronizado();
        
        Thread[] threads = new Thread[10];
        for (int i = 0; i < threads.length; i++) {
            threads[i] = new Thread(() -> {
                for (int j = 0; j < 1000; j++) {
                    contador.incrementar();
                }
            });
        }
        
        for (Thread t : threads) {
            t.start();
        }
        
        for (Thread t : threads) {
            try {
                t.join();
            } catch (InterruptedException e) {
                e.printStackTrace();
            }
        }
        
        System.out.println("Valor esperado: 10000");
        System.out.println("Valor real: " + contador.getValor());
        System.out.println("Sincronização resolveu o problema!");
    }
    
    public static void demonstrarLocks() {
        System.out.println("\n=== LOCKS EXPLÍCITOS ===");
        
        class ContadorComLock {
            private int valor = 0;
            private final Lock lock = new ReentrantLock();
            
            public void incrementar() {
                lock.lock(); // Adquire o lock
                try {
                    valor++;
                } finally {
                    lock.unlock(); // Libera o lock no finally
                }
            }
            
            public int getValor() {
                lock.lock();
                try {
                    return valor;
                } finally {
                    lock.unlock();
                }
            }
        }
        
        ContadorComLock contador = new ContadorComLock();
        
        // Testando com tryLock
        Thread t1 = new Thread(() -> {
            for (int i = 0; i < 5; i++) {
                if (contador.lock.tryLock()) {
                    try {
                        System.out.println(Thread.currentThread().getName() + " adquiriu o lock");
                        Thread.sleep(1000);
                        contador.incrementar();
                    } catch (InterruptedException e) {
                        e.printStackTrace();
                    } finally {
                        contador.lock.unlock();
                    }
                } else {
                    System.out.println(Thread.currentThread().getName() + " não conseguiu o lock, tentando novamente...");
                    try {
                        Thread.sleep(500);
                    } catch (InterruptedException e) {
                        e.printStackTrace();
                    }
                }
            }
        }, "Thread-TryLock");
        
        Thread t2 = new Thread(() -> {
            for (int i = 0; i < 5; i++) {
                contador.incrementar();
                try {
                    Thread.sleep(300);
                } catch (InterruptedException e) {
                    e.printStackTrace();
                }
            }
        }, "Thread-Normal");
        
        t1.start();
        t2.start();
        
        try {
            t1.join();
            t2.join();
        } catch (InterruptedException e) {
            e.printStackTrace();
        }
        
        System.out.println("Valor final: " + contador.getValor());
        
        // ReadWriteLock para múltiplos leitores e um escritor
        demonstrarReadWriteLock();
    }
    
    public static void demonstrarReadWriteLock() {
        System.out.println("\n=== READWRITELOCK ===");
        
        class DadosCompartilhados {
            private String dados = "Valor inicial";
            private final ReadWriteLock rwLock = new ReentrantReadWriteLock();
            private final Lock readLock = rwLock.readLock();
            private final Lock writeLock = rwLock.writeLock();
            
            public String ler() {
                readLock.lock();
                try {
                    System.out.println(Thread.currentThread().getName() + " lendo: " + dados);
                    Thread.sleep(100); // Simula tempo de leitura
                    return dados;
                } catch (InterruptedException e) {
                    return null;
                } finally {
                    readLock.unlock();
                }
            }
            
            public void escrever(String novoValor) {
                writeLock.lock();
                try {
                    System.out.println(Thread.currentThread().getName() + " escrevendo: " + novoValor);
                    Thread.sleep(500); // Simula tempo de escrita
                    dados = novoValor;
                } catch (InterruptedException e) {
                    e.printStackTrace();
                } finally {
                    writeLock.unlock();
                }
            }
        }
        
        DadosCompartilhados dados = new DadosCompartilhados();
        
        // Múltiplos leitores
        for (int i = 0; i < 3; i++) {
            new Thread(() -> {
                for (int j = 0; j < 3; j++) {
                    dados.ler();
                }
            }, "Leitor-" + i).start();
        }
        
        // Um escritor
        new Thread(() -> {
            for (int i = 0; i < 2; i++) {
                dados.escrever("Novo valor " + i);
            }
        }, "Escritor").start();
        
        try {
            Thread.sleep(5000);
        } catch (InterruptedException e) {
            e.printStackTrace();
        }
    }
    
    public static void demonstrarDeadlock() {
        System.out.println("\n=== DEADLOCK ===");
        
        class Recurso {
            private String nome;
            
            public Recurso(String nome) {
                this.nome = nome;
            }
            
            public String getNome() {
                return nome;
            }
            
            public synchronized void usar(Recurso outro) {
                System.out.println(Thread.currentThread().getName() + " usando " + nome);
                try {
                    Thread.sleep(100);
                } catch (InterruptedException e) {}
                
                System.out.println(Thread.currentThread().getName() + " tentando usar " + outro.getNome());
                outro.usar(this); // Potencial deadlock!
            }
            
            public synchronized void usarSeguro(Recurso outro) {
                // Evita deadlock adquirindo locks em ordem consistente
                Recurso primeiro = this.hashCode() < outro.hashCode() ? this : outro;
                Recurso segundo = this.hashCode() < outro.hashCode() ? outro : this;
                
                synchronized (primeiro) {
                    synchronized (segundo) {
                        System.out.println(Thread.currentThread().getName() + " usando " + nome + " e " + outro.getNome());
                        try {
                            Thread.sleep(100);
                        } catch (InterruptedException e) {}
                    }
                }
            }
        }
        
        Recurso recursoA = new Recurso("A");
        Recurso recursoB = new Recurso("B");
        
        // Thread 1: A -> B
        Thread t1 = new Thread(() -> {
            recursoA.usar(recursoB); // Causa deadlock
        }, "Thread-1");
        
        // Thread 2: B -> A  
        Thread t2 = new Thread(() -> {
            recursoB.usar(recursoA); // Causa deadlock
        }, "Thread-2");
        
        t1.start();
        t2.start();
        
        // Aguarda um tempo e verifica se as threads estão presas
        try {
            Thread.sleep(2000);
            
            if (t1.isAlive() && t2.isAlive()) {
                System.out.println("DEADLOCK DETECTADO!");
                System.out.println("Estado t1: " + t1.getState());
                System.out.println("Estado t2: " + t2.getState());
                
                // Tentativa de recuperação (não recomendado em produção)
                t1.interrupt();
                t2.interrupt();
            }
        } catch (InterruptedException e) {
            e.printStackTrace();
        }
        
        // Versão segura sem deadlock
        System.out.println("\nVersão segura sem deadlock:");
        Thread t3 = new Thread(() -> {
            recursoA.usarSeguro(recursoB);
        }, "Thread-Segura-1");
        
        Thread t4 = new Thread(() -> {
            recursoB.usarSeguro(recursoA);
        }, "Thread-Segura-2");
        
        t3.start();
        t4.start();
        
        try {
            t3.join();
            t4.join();
        } catch (InterruptedException e) {
            e.printStackTrace();
        }
    }
    
    public static void demonstrarWaitNotify() {
        System.out.println("\n=== WAIT E NOTIFY ===");
        
        class Buffer {
            private String mensagem;
            private boolean vazio = true;
            
            public synchronized String consumir() {
                while (vazio) {
                    try {
                        System.out.println(Thread.currentThread().getName() + " esperando mensagem...");
                        wait(); // Libera o lock e espera
                    } catch (InterruptedException e) {
                        e.printStackTrace();
                    }
                }
                vazio = true;
                System.out.println(Thread.currentThread().getName() + " consumiu: " + mensagem);
                notifyAll(); // Notifica produtores
                return mensagem;
            }
            
            public synchronized void produzir(String mensagem) {
                while (!vazio) {
                    try {
                        System.out.println(Thread.currentThread().getName() + " esperando espaço...");
                        wait(); // Libera o lock e espera
                    } catch (InterruptedException e) {
                        e.printStackTrace();
                    }
                }
                this.mensagem = mensagem;
                vazio = false;
                System.out.println(Thread.currentThread().getName() + " produziu: " + mensagem);
                notifyAll(); // Notifica consumidores
            }
        }
        
        Buffer buffer = new Buffer();
        
        // Produtor
        Thread produtor = new Thread(() -> {
            String[] mensagens = {"Mensagem 1", "Mensagem 2", "Mensagem 3", "FIM"};
            for (String msg : mensagens) {
                buffer.produzir(msg);
                try {
                    Thread.sleep(1000);
                } catch (InterruptedException e) {
                    e.printStackTrace();
                }
            }
        }, "Produtor");
        
        // Consumidor
        Thread consumidor = new Thread(() -> {
            String mensagem;
            do {
                mensagem = buffer.consumir();
                try {
                    Thread.sleep(1500);
                } catch (InterruptedException e) {
                    e.printStackTrace();
                }
            } while (!"FIM".equals(mensagem));
            System.out.println("Consumidor terminou");
        }, "Consumidor");
        
        produtor.start();
        consumidor.start();
        
        try {
            produtor.join();
            consumidor.join();
        } catch (InterruptedException e) {
            e.printStackTrace();
        }
    }
}
```

### **11.2.3 Framework Executor**

**Exemplo 11.3: Gerenciamento de Threads com Executor Framework**

```java
import java.util.concurrent.*;
import java.util.*;

public class ExemploExecutor {

    public static void main(String[] args) {
        System.out.println("=== FRAMEWORK EXECUTOR ===");
        
        // Executors básicos
        demonstrarExecutorsBasicos();
        
        // ThreadPoolExecutor
        demonstrarThreadPool();
        
        // ScheduledExecutorService
        demonstrarAgendamento();
        
        // ForkJoinPool
        demonstrarForkJoin();
        
        // CompletableFuture
        demonstrarCompletableFuture();
    }
    
    public static void demonstrarExecutorsBasicos() {
        System.out.println("\n=== EXECUTORS BÁSICOS ===");
        
        // SingleThreadExecutor - Uma única thread
        ExecutorService singleThread = Executors.newSingleThreadExecutor();
        
        singleThread.execute(() -> {
            System.out.println("Tarefa 1 executando em: " + Thread.currentThread().getName());
        });
        
        singleThread.execute(() -> {
            System.out.println("Tarefa 2 executando em: " + Thread.currentThread().getName());
        });
        
        // CachedThreadPool - Threads sob demanda
        ExecutorService cachedPool = Executors.newCachedThreadPool();
        
        for (int i = 0; i < 5; i++) {
            final int taskId = i;
            cachedPool.submit(() -> {
                System.out.println("Tarefa " + taskId + " em: " + Thread.currentThread().getName());
                try {
                    Thread.sleep(1000);
                } catch (InterruptedException e) {
                    e.printStackTrace();
                }
            });
        }
        
        // FixedThreadPool - Pool fixo de threads
        ExecutorService fixedPool = Executors.newFixedThreadPool(3);
        
        List<Future<String>> futures = new ArrayList<>();
        for (int i = 0; i < 6; i++) {
            final int taskId = i;
            Future<String> future = fixedPool.submit(() -> {
                System.out.println("Tarefa fixa " + taskId + " em: " + Thread.currentThread().getName());
                Thread.sleep(500);
                return "Resultado da tarefa " + taskId;
            });
            futures.add(future);
        }
        
        // Coletando resultados
        futures.forEach(f -> {
            try {
                System.out.println("Resultado: " + f.get());
            } catch (Exception e) {
                e.printStackTrace();
            }
        });
        
        // Shutdown dos executors
        singleThread.shutdown();
        cachedPool.shutdown();
        fixedPool.shutdown();
        
        try {
            // Aguarda término com timeout
            if (!fixedPool.awaitTermination(5, TimeUnit.SECONDS)) {
                System.out.println("Forçando shutdown...");
                fixedPool.shutdownNow();
            }
        } catch (InterruptedException e) {
            fixedPool.shutdownNow();
        }
    }
    
    public static void demonstrarThreadPool() {
        System.out.println("\n=== THREADPOOLEXECUTOR ===");
        
        // Criando ThreadPoolExecutor customizado
        ThreadPoolExecutor customExecutor = new ThreadPoolExecutor(
            2, // corePoolSize
            4, // maximumPoolSize  
            60, // keepAliveTime
            TimeUnit.SECONDS, // unit
            new ArrayBlockingQueue<>(10), // workQueue
            Executors.defaultThreadFactory(), // threadFactory
            new ThreadPoolExecutor.CallerRunsPolicy() // rejectionHandler
        );
        
        // Monitorando o executor
        ScheduledExecutorService monitor = Executors.newScheduledThreadPool(1);
        monitor.scheduleAtFixedRate(() -> {
            System.out.printf("Pool: [Tarefas: %d, Ativas: %d, Concluídas: %d, Fila: %d]%n",
                customExecutor.getTaskCount(),
                customExecutor.getActiveCount(),
                customExecutor.getCompletedTaskCount(),
                customExecutor.getQueue().size());
        }, 0, 1, TimeUnit.SECONDS);
        
        // Submetendo tarefas
        for (int i = 0; i < 15; i++) {
            final int taskId = i;
            try {
                customExecutor.execute(() -> {
                    System.out.println("Tarefa " + taskId + " executando em: " + Thread.currentThread().getName());
                    try {
                        Thread.sleep(2000);
                    } catch (InterruptedException e) {
                        Thread.currentThread().interrupt();
                    }
                });
            } catch (RejectedExecutionException e) {
                System.out.println("Tarefa " + taskId + " rejeitada!");
            }
        }
        
        // Shutdown
        customExecutor.shutdown();
        try {
            if (!customExecutor.awaitTermination(10, TimeUnit.SECONDS)) {
                customExecutor.shutdownNow();
            }
        } catch (InterruptedException e) {
            customExecutor.shutdownNow();
        }
        
        monitor.shutdown();
    }
    
    public static void demonstrarAgendamento() {
        System.out.println("\n=== SCHEDULEDEXECUTORSERVICE ===");
        
        ScheduledExecutorService scheduler = Executors.newScheduledThreadPool(2);
        
        // Tarefa com delay fixo
        ScheduledFuture<?> tarefaFixa = scheduler.schedule(() -> {
            System.out.println("Tarefa única executada após 2 segundos");
        }, 2, TimeUnit.SECONDS);
        
        // Tarefa periódica com rate fixo
        scheduler.scheduleAtFixedRate(() -> {
            System.out.println("Tarefa rate-fixed: " + new Date());
        }, 1, 2, TimeUnit.SECONDS);
        
        // Tarefa periódica com delay entre término e próximo início
        scheduler.scheduleWithFixedDelay(() -> {
            System.out.println("Tarefa fixed-delay iniciada");
            try {
                Thread.sleep(1000); // Simula trabalho
            } catch (InterruptedException e) {
                e.printStackTrace();
            }
            System.out.println("Tarefa fixed-delay concluída");
        }, 1, 2, TimeUnit.SECONDS);
        
        // Executa por 10 segundos e depois cancela
        try {
            Thread.sleep(10000);
        } catch (InterruptedException e) {
            e.printStackTrace();
        }
        
        scheduler.shutdown();
        System.out.println("Scheduler finalizado");
    }
    
    public static void demonstrarForkJoin() {
        System.out.println("\n=== FORKJOINPOOL ===");
        
        // Exemplo: Soma de array grande
        int[] array = new int[1000];
        Arrays.fill(array, 1);
        
        ForkJoinPool forkJoinPool = ForkJoinPool.commonPool();
        
        SomaArrayTask task = new SomaArrayTask(array, 0, array.length);
        Long resultado = forkJoinPool.invoke(task);
        
        System.out.println("Soma do array: " + resultado);
        System.out.println("Parallelismo: " + forkJoinPool.getParallelism());
        System.out.println("Pool size: " + forkJoinPool.getPoolSize());
    }
    
    static class SomaArrayTask extends RecursiveTask<Long> {
        private static final int LIMITE = 100;
        private final int[] array;
        private final int inicio;
        private final int fim;
        
        public SomaArrayTask(int[] array, int inicio, int fim) {
            this.array = array;
            this.inicio = inicio;
            this.fim = fim;
        }
        
        @Override
        protected Long compute() {
            int tamanho = fim - inicio;
            if (tamanho <= LIMITE) {
                // Computação direta
                long soma = 0;
                for (int i = inicio; i < fim; i++) {
                    soma += array[i];
                }
                return soma;
            } else {
                // Divide e conquista
                int meio = inicio + (tamanho / 2);
                SomaArrayTask esquerda = new SomaArrayTask(array, inicio, meio);
                SomaArrayTask direita = new SomaArrayTask(array, meio, fim);
                
                esquerda.fork(); // Executa em outra thread
                Long resultadoDireita = direita.compute(); // Computa na thread atual
                Long resultadoEsquerda = esquerda.join(); // Aguarda resultado da outra thread
                
                return resultadoEsquerda + resultadoDireita;
            }
        }
    }
    
    public static void demonstrarCompletableFuture() {
        System.out.println("\n=== COMPLETABLEFUTURE ===");
        
        // Criação básica
        CompletableFuture<String> futuro1 = CompletableFuture.supplyAsync(() -> {
            System.out.println("Executando supplyAsync em: " + Thread.currentThread().getName());
            try {
                Thread.sleep(1000);
            } catch (InterruptedException e) {
                throw new IllegalStateException(e);
            }
            return "Resultado do supplyAsync";
        });
        
        // Encadeamento com thenApply
        CompletableFuture<String> futuro2 = futuro1.thenApply(resultado -> {
            System.out.println("Processando resultado: " + resultado);
            return resultado.toUpperCase();
        });
        
        // Encadeamento com thenAccept
        futuro2.thenAccept(resultado -> {
            System.out.println("Consumindo resultado: " + resultado);
        });
        
        // Combinação de futures
        CompletableFuture<String> futuro3 = CompletableFuture.supplyAsync(() -> {
            try {
                Thread.sleep(500);
            } catch (InterruptedException e) {
                e.printStackTrace();
            }
            return "Future 3";
        });
        
        CompletableFuture<String> futuro4 = CompletableFuture.supplyAsync(() -> {
            try {
                Thread.sleep(300);
            } catch (InterruptedException e) {
                e.printStackTrace();
            }
            return "Future 4";
        });
        
        CompletableFuture<String> combinado = futuro3.thenCombine(futuro4, (r3, r4) -> {
            return r3 + " + " + r4;
        });
        
        // Tratamento de exceções
        CompletableFuture<String> futuroComErro = CompletableFuture.supplyAsync(() -> {
            if (true) {
                throw new RuntimeException("Erro simulado!");
            }
            return "Sucesso";
        }).exceptionally(erro -> {
            System.out.println("Tratando erro: " + erro.getMessage());
            return "Valor padrão em caso de erro";
        });
        
        // Múltiplos futures
        List<CompletableFuture<String>> futures = Arrays.asList(
            CompletableFuture.supplyAsync(() -> "A"),
            CompletableFuture.supplyAsync(() -> "B"),
            CompletableFuture.supplyAsync(() -> "C")
        );
        
        CompletableFuture<Void> todos = CompletableFuture.allOf(
            futures.toArray(new CompletableFuture[0])
        );
        
        CompletableFuture<List<String>> resultados = todos.thenApply(v ->
            futures.stream()
                .map(CompletableFuture::join)
                .collect(Collectors.toList())
        );
        
        // Aguarda conclusão
        try {
            System.out.println("Resultado combinado: " + combinado.get());
            System.out.println("Future com erro: " + futuroComErro.get());
            System.out.println("Todos resultados: " + resultados.get());
        } catch (Exception e) {
            e.printStackTrace();
        }
    }
}
```

### **11.2.4 Coleções Thread-Safe**

**Exemplo 11.4: Coleções Concorrentes**

```java
import java.util.*;
import java.util.concurrent.*;

public class ExemploColecoesConcorrentes {

    public static void main(String[] args) {
        System.out.println("=== COLEÇÕES THREAD-SAFE ===");
        
        // ConcurrentHashMap
        demonstrarConcurrentHashMap();
        
        // CopyOnWriteArrayList
        demonstrarCopyOnWrite();
        
        // BlockingQueue
        demonstrarBlockingQueue();
        
        // ConcurrentLinkedQueue
        demonstrarConcurrentLinkedQueue();
        
        // Coleções sincronizadas
        demonstrarColecoesSincronizadas();
    }
    
    public static void demonstrarConcurrentHashMap() {
        System.out.println("\n=== CONCURRENTHASHMAP ===");
        
        ConcurrentHashMap<String, Integer> map = new ConcurrentHashMap<>();
        
        // Operações atômicas
        map.put("chave1", 1);
        map.putIfAbsent("chave1", 100); // Não substitui
        map.putIfAbsent("chave2", 2);   // Adiciona
        
        System.out.println("Map: " + map);
        
        // Compute operations
        map.compute("chave1", (k, v) -> v + 10);
        map.computeIfAbsent("chave3", k -> 3);
        map.computeIfPresent("chave2", (k, v) -> v * 2);
        
        System.out.println("Após computações: " + map);
        
        // Operações em lote
        map.forEach(2, (k, v) -> System.out.println(k + " -> " + v));
        
        // Reduce
        Integer soma = map.reduceValues(2, Integer::sum);
        System.out.println("Soma dos valores: " + soma);
        
        // Search
        String resultado = map.search(2, (k, v) -> v > 2 ? k : null);
        System.out.println("Primeira chave com valor > 2: " + resultado);
        
        // Teste de concorrência
        testarConcorrenciaHashMap();
    }
    
    public static void testarConcorrenciaHashMap() {
        System.out.println("\n--- Teste de Concorrência ---");
        
        ConcurrentHashMap<String, Integer> map = new ConcurrentHashMap<>();
        ExecutorService executor = Executors.newFixedThreadPool(4);
        
        // Múltiplas threads escrevendo
        for (int i = 0; i < 10; i++) {
            final int threadId = i;
            executor.execute(() -> {
                for (int j = 0; j < 100; j++) {
                    String chave = "thread-" + threadId + "-" + j;
                    map.put(chave, threadId * 100 + j);
                }
            });
        }
        
        // Thread lendo enquanto outras escrevem
        executor.execute(() -> {
            while (map.size() < 1000) {
                System.out.println("Tamanho atual: " + map.size());
                try {
                    Thread.sleep(100);
                } catch (InterruptedException e) {
                    break;
                }
            }
        });
        
        executor.shutdown();
        try {
            executor.awaitTermination(5, TimeUnit.SECONDS);
        } catch (InterruptedException e) {
            e.printStackTrace();
        }
        
        System.out.println("Tamanho final: " + map.size());
    }
    
    public static void demonstrarCopyOnWrite() {
        System.out.println("\n=== COPYONWRITEARRAYLIST ===");
        
        CopyOnWriteArrayList<String> lista = new CopyOnWriteArrayList<>();
        
        // Adiciona elementos
        lista.add("A");
        lista.add("B");
        lista.add("C");
        
        System.out.println("Lista inicial: " + lista);
        
        // Iteração thread-safe (usa snapshot)
        new Thread(() -> {
            Iterator<String> it = lista.iterator();
            while (it.hasNext()) {
                System.out.println("Thread 1 lendo: " + it.next());
                try {
                    Thread.sleep(100);
                } catch (InterruptedException e) {
                    break;
                }
            }
        }).start();
        
        // Modificação durante iteração (não afeta iteração atual)
        new Thread(() -> {
            try {
                Thread.sleep(50);
                lista.add("D");
                System.out.println("Thread 2 adicionou D");
                
                Thread.sleep(100);
                lista.remove("A");
                System.out.println("Thread 2 removeu A");
            } catch (InterruptedException e) {
                e.printStackTrace();
            }
        }).start();
        
        try {
            Thread.sleep(500);
        } catch (InterruptedException e) {
            e.printStackTrace();
        }
        
        System.out.println("Lista final: " + lista);
        
        // CopyOnWriteArraySet
        CopyOnWriteArraySet<String> set = new CopyOnWriteArraySet<>();
        set.add("X");
        set.add("Y");
        set.add("X"); // Duplicado ignorado
        
        System.out.println("Set: " + set);
    }
    
    public static void demonstrarBlockingQueue() {
        System.out.println("\n=== BLOCKINGQUEUE ===");
        
        // ArrayBlockingQueue
        BlockingQueue<String> queue = new ArrayBlockingQueue<>(5);
        
        // Produtor
        Thread produtor = new Thread(() -> {
            String[] mensagens = {"M1", "M2", "M3", "M4", "M5", "M6"};
            for (String msg : mensagens) {
                try {
                    boolean inserido = queue.offer(msg, 1, TimeUnit.SECONDS);
                    if (inserido) {
                        System.out.println("Produzido: " + msg);
                    } else {
                        System.out.println("Fila cheia, não pôde produzir: " + msg);
                    }
                    Thread.sleep(200);
                } catch (InterruptedException e) {
                    break;
                }
            }
        });
        
        // Consumidor
        Thread consumidor = new Thread(() -> {
            while (true) {
                try {
                    String mensagem = queue.poll(2, TimeUnit.SECONDS);
                    if (mensagem == null) {
                        System.out.println("Timeout - nenhuma mensagem disponível");
                        break;
                    }
                    System.out.println("Consumido: " + mensagem);
                    Thread.sleep(300);
                } catch (InterruptedException e) {
                    break;
                }
            }
        });
        
        produtor.start();
        consumidor.start();
        
        try {
            produtor.join();
            Thread.sleep(1000); // Aguarda processamento
            consumidor.interrupt();
            consumidor.join();
        } catch (InterruptedException e) {
            e.printStackTrace();
        }
        
        // LinkedBlockingQueue
        BlockingQueue<Integer> linkedQueue = new LinkedBlockingQueue<>(3);
        
        // PriorityBlockingQueue
        BlockingQueue<Integer> priorityQueue = new PriorityBlockingQueue<>(5, Comparator.reverseOrder());
        
        priorityQueue.add(3);
        priorityQueue.add(1);
        priorityQueue.add(4);
        priorityQueue.add(2);
        
        System.out.println("PriorityQueue ordenado:");
        while (!priorityQueue.isEmpty()) {
            try {
                System.out.println(priorityQueue.take());
            } catch (InterruptedException e) {
                e.printStackTrace();
            }
        }
    }
    
    public static void demonstrarConcurrentLinkedQueue() {
        System.out.println("\n=== CONCURRENTLINKEDQUEUE ===");
        
        ConcurrentLinkedQueue<String> queue = new ConcurrentLinkedQueue<>();
        
        // Múltiplos produtores
        ExecutorService produtores = Executors.newFixedThreadPool(3);
        for (int i = 0; i < 10; i++) {
            final int taskId = i;
            produtores.execute(() -> {
                queue.offer("Mensagem-" + taskId);
                System.out.println("Produzido: Mensagem-" + taskId);
            });
        }
        
        // Múltiplos consumidores
        ExecutorService consumidores = Executors.newFixedThreadPool(2);
        for (int i = 0; i < 10; i++) {
            consumidores.execute(() -> {
                String mensagem = queue.poll();
                if (mensagem != null) {
                    System.out.println("Consumido: " + mensagem);
                }
            });
        }
        
        produtores.shutdown();
        consumidores.shutdown();
        
        try {
            produtores.awaitTermination(2, TimeUnit.SECONDS);
            consumidores.awaitTermination(2, TimeUnit.SECONDS);
        } catch (InterruptedException e) {
            e.printStackTrace();
        }
        
        System.out.println("Fila final: " + queue);
    }
    
    public static void demonstrarColecoesSincronizadas() {
        System.out.println("\n=== COLEÇÕES SINCRONIZADAS ===");
        
        // Lista sincronizada
        List<String> listaSincronizada = Collections.synchronizedList(new ArrayList<>());
        
        // Map sincronizado
        Map<String, Integer> mapSincronizado = Collections.synchronizedMap(new HashMap<>());
        
        // Set sincronizado
        Set<String> setSincronizado = Collections.synchronizedSet(new HashSet<>());
        
        // Teste com múltiplas threads
        ExecutorService executor = Executors.newFixedThreadPool(4);
        
        for (int i = 0; i < 10; i++) {
            final int taskId = i;
            executor.execute(() -> {
                listaSincronizada.add("Task-" + taskId);
                mapSincronizado.put("Key-" + taskId, taskId);
                setSincronizado.add("Value-" + taskId);
            });
        }
        
        executor.shutdown();
        try {
            executor.awaitTermination(2, TimeUnit.SECONDS);
        } catch (InterruptedException e) {
            e.printStackTrace();
        }
        
        System.out.println("Lista sincronizada: " + listaSincronizada);
        System.out.println("Map sincronizado: " + mapSincronizado);
        System.out.println("Set sincronizado: " + setSincronizado);
        
        // Iteração segura em coleções sincronizadas
        synchronized (listaSincronizada) {
            Iterator<String> it = listaSincronizada.iterator();
            while (it.hasNext()) {
                System.out.println("Elemento: " + it.next());
            }
        }
    }
}
```

## **11.3 Exercícios Práticos**

### **Exercício 11.1: Sistema de Processamento de Pedidos**

```java
import java.util.concurrent.*;
import java.util.*;

public class SistemaPedidos {
    private final BlockingQueue<Pedido> filaPedidos;
    private final ExecutorService processadores;
    private volatile boolean executando = true;
    
    public SistemaPedidos(int capacidadeFila, int numProcessadores) {
        this.filaPedidos = new ArrayBlockingQueue<>(capacidadeFila);
        this.processadores = Executors.newFixedThreadPool(numProcessadores);
    }
    
    public void iniciar() {
        // Inicia processadores
        for (int i = 0; i < ((ThreadPoolExecutor)processadores).getCorePoolSize(); i++) {
            processadores.execute(this::processarPedido);
        }
        
        // Inicia monitoramento
        Executors.newSingleThreadScheduledExecutor().scheduleAtFixedRate(
            this::monitorarSistema, 1, 1, TimeUnit.SECONDS);
    }
    
    public void parar() {
        executando = false;
        processadores.shutdown();
        try {
            if (!processadores.awaitTermination(10, TimeUnit.SECONDS)) {
                processadores.shutdownNow();
            }
        } catch (InterruptedException e) {
            processadores.shutdownNow();
        }
    }
    
    public boolean submeterPedido(Pedido pedido) {
        return filaPedidos.offer(pedido);
    }
    
    private void processarPedido() {
        while (executando || !filaPedidos.isEmpty()) {
            try {
                Pedido pedido = filaPedidos.poll(1, TimeUnit.SECONDS);
                if (pedido != null) {
                    System.out.println("Processando pedido: " + pedido);
                    Thread.sleep(1000); // Simula processamento
                    System.out.println("Pedido concluído: " + pedido);
                }
            } catch (InterruptedException e) {
                Thread.currentThread().interrupt();
                break;
            }
        }
    }
    
    private void monitorarSistema() {
        System.out.printf("[Monitor] Fila: %d, Threads Ativas: %d%n",
            filaPedidos.size(),
            ((ThreadPoolExecutor)processadores).getActiveCount());
    }
    
    static class Pedido {
        private final String id;
        private final String cliente;
        private final double valor;
        
        public Pedido(String id, String cliente, double valor) {
            this.id = id;
            this.cliente = cliente;
            this.valor = valor;
        }
        
        @Override
        public String toString() {
            return String.format("Pedido{id=%s, cliente=%s, valor=%.2f}", id, cliente, valor);
        }
    }
    
    public static void main(String[] args) {
        SistemaPedidos sistema = new SistemaPedidos(100, 3);
        sistema.iniciar();
        
        // Simula submissão de pedidos
        Random random = new Random();
        for (int i = 0; i < 20; i++) {
            Pedido pedido = new Pedido("PED" + i, "Cliente" + i, random.nextDouble() * 1000);
            if (!sistema.submeterPedido(pedido)) {
                System.out.println("Fila cheia, pedido rejeitado: " + pedido);
            }
            try {
                Thread.sleep(200);
            } catch (InterruptedException e) {
                e.printStackTrace();
            }
        }
        
        // Aguarda processamento e para o sistema
        try {
            Thread.sleep(5000);
        } catch (InterruptedException e) {
            e.printStackTrace();
        }
        
        sistema.parar();
    }
}
```

## **11.4 Questionário de Revisão**

**Questão 1:** Qual a diferença entre `Runnable` e `Callable`?
- A) `Runnable` não retorna valor, `Callable` retorna
- B) `Runnable` pode lançar exceções verificadas
- C) `Callable` não pode ser usado com ExecutorService

**Questão 2:** O que é race condition?
- A) Condição onde múltiplas threads acessam dados compartilhados simultaneamente
- B) Uma corrida entre threads para ver qual termina primeiro
- C) Um tipo de exceção em programação concorrente

**Questão 3:** Para que serve o `volatile` em Java?
- A) Garante visibilidade de mudanças entre threads
- B) Substitui a necessidade de sincronização
- C) Acelera o acesso à variável

**Questão 4:** Qual a vantagem do `ConcurrentHashMap` sobre `Collections.synchronizedMap()`?
- A) Melhor performance em leituras concorrentes
- B) Não permite valores nulos
- C) Ambas as anteriores

**Questão 5:** O que é um `CompletableFuture`?

## **11.5 Laboratório Prático**

**Projeto: Sistema de Cache Distribuído**

```java
// Implemente um sistema de cache distribuído com:
// 1. Cache com tempo de expiração
// 2. Limpeza automática de entradas expiradas
// 3. Estatísticas de uso (hits/misses)
// 4. Suporte a operações em lote
// 5. Backup e recuperação do cache

// Use ConcurrentHashMap, ScheduledExecutorService, e outras classes concorrentes
```

## **11.6 Material de Apoio**

**Resumo dos Principais Componentes:**

**Threads:**
- `Thread`, `Runnable`, `Callable`
- Estados: NEW, RUNNABLE, BLOCKED, WAITING, TIMED_WAITING, TERMINATED

**Sincronização:**
- `synchronized` (métodos e blocos)
- `Lock`, `ReentrantLock`, `ReadWriteLock`
- `volatile`, `AtomicInteger`, `AtomicReference`

**Executors:**
- `ExecutorService`, `ThreadPoolExecutor`, `ScheduledExecutorService`
- `ForkJoinPool`, `RecursiveTask`, `RecursiveAction`

**Coleções Concorrentes:**
- `ConcurrentHashMap`, `ConcurrentSkipListMap`
- `CopyOnWriteArrayList`, `CopyOnWriteArraySet`
- `BlockingQueue`, `ConcurrentLinkedQueue`

**Futures:**
- `Future`, `CompletableFuture`
- `FutureTask`

**Padrões Comuns:**
- Producer-Consumer (BlockingQueue)
- Thread Pool (ExecutorService)
- Fork-Join (ForkJoinPool)
- Monitor Object (synchronized)
- Double-Checked Locking

**Dicas Importantes:**
- Prefira `ExecutorService` sobre `Thread` diretamente
- Use `ConcurrentHashMap` para maps compartilhados
- `volatile` para flags de controle entre threads
- Sempre libere locks em blocos `finally`
- Use `ThreadLocal` para dados por-thread
- Evite deadlocks adquirindo locks em ordem consistente
- Teste extensivamente em ambiente multi-thread

---

# **Módulo 12: I/O e NIO.2**

## **12.1 Objetivos do Módulo**

- Dominar as operações básicas de I/O com streams
- Compreender a hierarquia de classes de I/O do Java
- Aprender a usar a API NIO.2 para operações de arquivos
- Trabalhar com caminhos, arquivos e diretórios
- Implementar operações de leitura e escrita eficientes
- Entender o uso de buffers e channels

## **12.2 Conteúdo Programático**

### **12.2.1 Fundamentos de I/O com Streams**

**Exemplo 12.1: Operações Básicas com FileInputStream e FileOutputStream**

```java
import java.io.*;
import java.util.*;

public class ExemploIOBasico {

    public static void main(String[] args) {
        System.out.println("=== FUNDAMENTOS DE I/O ===");
        
        // Operações com File
        demonstrarFile();
        
        // InputStream e OutputStream
        demonstrarStreams();
        
        // Reader e Writer
        demonstrarReadersWriters();
        
        // Buffered streams
        demonstrarBufferedStreams();
    }
    
    public static void demonstrarFile() {
        System.out.println("\n=== CLASSE FILE ===");
        
        // Criando objeto File
        File arquivo = new File("exemplo.txt");
        File diretorio = new File("meu_diretorio");
        
        try {
            // Operações com arquivo
            System.out.println("Nome do arquivo: " + arquivo.getName());
            System.out.println("Caminho absoluto: " + arquivo.getAbsolutePath());
            System.out.println("Existe? " + arquivo.exists());
            System.out.println("É arquivo? " + arquivo.isFile());
            System.out.println("É diretório? " + arquivo.isDirectory());
            System.out.println("Tamanho: " + arquivo.length() + " bytes");
            System.out.println("Pode ler? " + arquivo.canRead());
            System.out.println("Pode escrever? " + arquivo.canWrite());
            System.out.println("Última modificação: " + new Date(arquivo.lastModified()));
            
            // Criando diretório
            if (diretorio.mkdir()) {
                System.out.println("Diretório criado: " + diretorio.getAbsolutePath());
            }
            
            // Listando arquivos
            File diretorioAtual = new File(".");
            System.out.println("\nConteúdo do diretório atual:");
            String[] arquivos = diretorioAtual.list();
            if (arquivos != null) {
                for (String nome : arquivos) {
                    System.out.println("  " + nome);
                }
            }
            
            // Operações de criação e exclusão
            if (arquivo.createNewFile()) {
                System.out.println("Arquivo criado: " + arquivo.getName());
            }
            
            // Renomear
            File novoArquivo = new File("exemplo_renomeado.txt");
            if (arquivo.renameTo(novoArquivo)) {
                System.out.println("Arquivo renomeado para: " + novoArquivo.getName());
            }
            
            // Excluir
            if (novoArquivo.delete()) {
                System.out.println("Arquivo excluído: " + novoArquivo.getName());
            }
            
        } catch (IOException e) {
            System.out.println("Erro nas operações de arquivo: " + e.getMessage());
        }
    }
    
    public static void demonstrarStreams() {
        System.out.println("\n=== INPUTSTREAM E OUTPUTSTREAM ===");
        
        // Escrevendo dados binários
        try (FileOutputStream fos = new FileOutputStream("dados.bin")) {
            byte[] dados = {65, 66, 67, 68, 69, 70}; // A-F em ASCII
            fos.write(dados);
            System.out.println("Dados binários escritos no arquivo");
            
            // Escrevendo string como bytes
            String texto = "Hello, World!";
            fos.write(texto.getBytes());
            System.out.println("Texto escrito como bytes");
            
        } catch (IOException e) {
            System.out.println("Erro ao escrever: " + e.getMessage());
        }
        
        // Lendo dados binários
        try (FileInputStream fis = new FileInputStream("dados.bin")) {
            System.out.println("Lendo dados binários:");
            
            // Lendo byte por byte
            int byteLido;
            while ((byteLido = fis.read()) != -1) {
                System.out.print((char) byteLido + "(" + byteLido + ") ");
            }
            System.out.println();
            
        } catch (IOException e) {
            System.out.println("Erro ao ler: " + e.getMessage());
        }
        
        // Leitura com buffer de bytes
        try (FileInputStream fis = new FileInputStream("dados.bin")) {
            byte[] buffer = new byte[1024];
            int bytesLidos;
            
            System.out.println("Lendo com buffer:");
            while ((bytesLidos = fis.read(buffer)) != -1) {
                String conteudo = new String(buffer, 0, bytesLidos);
                System.out.println("Bytes lidos: " + bytesLidos);
                System.out.println("Conteúdo: " + conteudo);
            }
            
        } catch (IOException e) {
            System.out.println("Erro na leitura com buffer: " + e.getMessage());
        }
    }
    
    public static void demonstrarReadersWriters() {
        System.out.println("\n=== READER E WRITER ===");
        
        // Escrevendo texto
        try (FileWriter writer = new FileWriter("texto.txt")) {
            writer.write("Linha 1: Olá, mundo!\n");
            writer.write("Linha 2: Programação Java\n");
            writer.write("Linha 3: I/O é fundamental\n");
            writer.write(String.format("Linha 4: Número formatado: %.2f%n", 3.14159));
            System.out.println("Texto escrito no arquivo");
            
        } catch (IOException e) {
            System.out.println("Erro ao escrever texto: " + e.getMessage());
        }
        
        // Lendo texto
        try (FileReader reader = new FileReader("texto.txt")) {
            System.out.println("Lendo texto caractere por caractere:");
            
            int charLido;
            while ((charLido = reader.read()) != -1) {
                System.out.print((char) charLido);
            }
            
        } catch (IOException e) {
            System.out.println("Erro ao ler texto: " + e.getMessage());
        }
        
        // Usando FileReader com char array
        try (FileReader reader = new FileReader("texto.txt")) {
            char[] buffer = new char[1024];
            int charsLidos;
            
            System.out.println("\nLendo texto com buffer de char:");
            while ((charsLidos = reader.read(buffer)) != -1) {
                String texto = new String(buffer, 0, charsLidos);
                System.out.print(texto);
            }
            
        } catch (IOException e) {
            System.out.println("Erro na leitura com buffer: " + e.getMessage());
        }
    }
    
    public static void demonstrarBufferedStreams() {
        System.out.println("\n=== BUFFERED STREAMS ===");
        
        // BufferedOutputStream - escrita eficiente
        try (BufferedOutputStream bos = new BufferedOutputStream(
             new FileOutputStream("buffered.bin"))) {
            
            for (int i = 0; i < 1000; i++) {
                bos.write(("Linha " + i + "\n").getBytes());
            }
            System.out.println("1000 linhas escritas com BufferedOutputStream");
            
        } catch (IOException e) {
            System.out.println("Erro na escrita buffered: " + e.getMessage());
        }
        
        // BufferedInputStream - leitura eficiente
        try (BufferedInputStream bis = new BufferedInputStream(
             new FileInputStream("buffered.bin"))) {
            
            byte[] buffer = new byte[1024];
            int bytesLidos;
            int totalBytes = 0;
            
            while ((bytesLidos = bis.read(buffer)) != -1) {
                totalBytes += bytesLidos;
            }
            System.out.println("Total de bytes lidos: " + totalBytes);
            
        } catch (IOException e) {
            System.out.println("Erro na leitura buffered: " + e.getMessage());
        }
        
        // BufferedReader - leitura de texto eficiente
        try (BufferedReader reader = new BufferedReader(
             new FileReader("texto.txt"))) {
            
            System.out.println("Lendo com BufferedReader:");
            String linha;
            int numeroLinha = 1;
            
            while ((linha = reader.readLine()) != null) {
                System.out.println(numeroLinha + ": " + linha);
                numeroLinha++;
            }
            
        } catch (IOException e) {
            System.out.println("Erro na leitura buffered: " + e.getMessage());
        }
        
        // BufferedWriter - escrita de texto eficiente
        try (BufferedWriter writer = new BufferedWriter(
             new FileWriter("buffered_text.txt"))) {
            
            for (int i = 1; i <= 5; i++) {
                writer.write("Esta é a linha " + i);
                writer.newLine(); // Escreve separador de linha
            }
            System.out.println("Texto escrito com BufferedWriter");
            
        } catch (IOException e) {
            System.out.println("Erro na escrita buffered: " + e.getMessage());
        }
    }
}
```

### **12.2.2 API NIO.2 (Java 7+)**

**Exemplo 12.2: Trabalhando com Path, Files e Diretórios**

```java
import java.nio.file.*;
import java.nio.charset.StandardCharsets;
import java.nio.ByteBuffer;
import java.nio.channels.*;
import java.io.IOException;
import java.util.*;
import java.util.stream.*;

public class ExemploNIO2 {

    public static void main(String[] args) {
        System.out.println("=== API NIO.2 ===");
        
        // Trabalhando com Path
        demonstrarPath();
        
        // Operações com Files
        demonstrarFiles();
        
        // Diretórios e walking
        demonstrarDiretorios();
        
        // FileChannel
        demonstrarFileChannel();
        
        // WatchService
        demonstrarWatchService();
    }
    
    public static void demonstrarPath() {
        System.out.println("\n=== CLASSE PATH ===");
        
        // Criando Paths
        Path path1 = Paths.get("exemplo.txt");
        Path path2 = Paths.get(".", "subdir", "arquivo.txt");
        Path path3 = Paths.get("/", "usr", "local", "bin");
        Path pathAbsoluto = Paths.get("C:", "Users", "joao", "documento.pdf");
        
        System.out.println("Path1: " + path1);
        System.out.println("Path2: " + path2);
        System.out.println("Path3: " + path3);
        System.out.println("Path absoluto: " + pathAbsoluto);
        
        // Operações com Path
        System.out.println("\n--- Operações com Path ---");
        System.out.println("Nome do arquivo: " + path1.getFileName());
        System.out.println("Diretório pai: " + path1.getParent());
        System.out.println("Raiz: " + path1.getRoot());
        System.out.println("É absoluto? " + path1.isAbsolute());
        System.out.println("Número de elementos: " + path2.getNameCount());
        
        // Elementos do path
        System.out.println("Elementos do path2:");
        for (int i = 0; i < path2.getNameCount(); i++) {
            System.out.println("  " + i + ": " + path2.getName(i));
        }
        
        // Resolvendo paths
        Path base = Paths.get("/base/diretorio");
        Path relativo = Paths.get("subdir/arquivo.txt");
        Path resolvido = base.resolve(relativo);
        System.out.println("Path resolvido: " + resolvido);
        
        // Normalizando
        Path complexo = Paths.get("./.././dir/../outrodir/arquivo.txt");
        Path normalizado = complexo.normalize();
        System.out.println("Path complexo: " + complexo);
        System.out.println("Path normalizado: " + normalizado);
        
        // Relativizando
        Path p1 = Paths.get("/home/user/documents");
        Path p2 = Paths.get("/home/user/documents/projects/java");
        Path relativo2 = p1.relativize(p2);
        System.out.println("Path relativo: " + relativo2);
    }
    
    public static void demonstrarFiles() {
        System.out.println("\n=== CLASSE FILES ===");
        
        try {
            // Verificando existência
            Path arquivo = Paths.get("arquivo_nio.txt");
            System.out.println("Existe? " + Files.exists(arquivo));
            System.out.println("Não existe? " + Files.notExists(arquivo));
            System.out.println("É legível? " + Files.isReadable(arquivo));
            System.out.println("É gravável? " + Files.isWritable(arquivo));
            System.out.println("É executável? " + Files.isExecutable(arquivo));
            System.out.println("É diretório? " + Files.isDirectory(arquivo));
            System.out.println("É arquivo regular? " + Files.isRegularFile(arquivo));
            System.out.println("É oculto? " + Files.isHidden(arquivo));
            
            // Criando arquivo
            if (!Files.exists(arquivo)) {
                Files.createFile(arquivo);
                System.out.println("Arquivo criado: " + arquivo);
            }
            
            // Escrevendo no arquivo
            List<String> linhas = Arrays.asList(
                "Linha 1: Introdução ao NIO.2",
                "Linha 2: Trabalhando com Path e Files",
                "Linha 3: Operações de I/O eficientes"
            );
            
            Files.write(arquivo, linhas, StandardCharsets.UTF_8);
            System.out.println("Dados escritos no arquivo");
            
            // Lendo todas as linhas
            System.out.println("\nConteúdo do arquivo:");
            List<String> conteudo = Files.readAllLines(arquivo, StandardCharsets.UTF_8);
            conteudo.forEach(System.out::println);
            
            // Lendo como string
            String todoConteudo = Files.readString(arquivo, StandardCharsets.UTF_8);
            System.out.println("\nConteúdo como string:");
            System.out.println(todoConteudo);
            
            // Atributos do arquivo
            System.out.println("\n--- Atributos do Arquivo ---");
            System.out.println("Tamanho: " + Files.size(arquivo) + " bytes");
            System.out.println("Última modificação: " + Files.getLastModifiedTime(arquivo));
            System.out.println("Proprietário: " + Files.getOwner(arquivo));
            
            // Copiando arquivo
            Path copia = Paths.get("copia_arquivo.txt");
            Files.copy(arquivo, copia, StandardCopyOption.REPLACE_EXISTING);
            System.out.println("Arquivo copiado para: " + copia);
            
            // Movendo/renomeando
            Path novoNome = Paths.get("arquivo_renomeado.txt");
            Files.move(arquivo, novoNome, StandardCopyOption.REPLACE_EXISTING);
            System.out.println("Arquivo movido para: " + novoNome);
            
            // Deletando
            Files.deleteIfExists(copia);
            Files.deleteIfExists(novoNome);
            System.out.println("Arquivos temporários removidos");
            
        } catch (IOException e) {
            System.out.println("Erro nas operações Files: " + e.getMessage());
        }
    }
    
    public static void demonstrarDiretorios() {
        System.out.println("\n=== DIRETÓRIOS ===");
        
        try {
            // Criando diretório
            Path diretorio = Paths.get("meu_diretorio_nio");
            if (!Files.exists(diretorio)) {
                Files.createDirectory(diretorio);
                System.out.println("Diretório criado: " + diretorio);
            }
            
            // Criando estrutura de diretórios
            Path estrutura = diretorio.resolve("subdir1/subdir2");
            Files.createDirectories(estrutura);
            System.out.println("Estrutura de diretórios criada: " + estrutura);
            
            // Criando alguns arquivos
            for (int i = 1; i <= 3; i++) {
                Path arquivo = diretorio.resolve("arquivo" + i + ".txt");
                Files.writeString(arquivo, "Conteúdo do arquivo " + i, 
                                StandardCharsets.UTF_8);
            }
            
            // Listando conteúdo do diretório
            System.out.println("\nConteúdo do diretório:");
            try (Stream<Path> stream = Files.list(diretorio)) {
                stream.forEach(path -> {
                    try {
                        String tipo = Files.isDirectory(path) ? "DIR" : "ARQ";
                        System.out.printf("  [%s] %s (size: %d)%n", 
                                        tipo, path.getFileName(), 
                                        Files.size(path));
                    } catch (IOException e) {
                        System.out.println("Erro ao acessar: " + path);
                    }
                });
            }
            
            // Walking pela árvore de diretórios
            System.out.println("\nÁrvore completa:");
            try (Stream<Path> stream = Files.walk(diretorio)) {
                stream.forEach(path -> {
                    int nivel = diretorio.relativize(path).getNameCount();
                    String indent = "  ".repeat(nivel);
                    String tipo = Files.isDirectory(path) ? "📁" : "📄";
                    System.out.println(indent + tipo + " " + path.getFileName());
                });
            }
            
            // Buscando arquivos com padrão
            System.out.println("\nBuscando arquivos .txt:");
            try (Stream<Path> stream = Files.find(diretorio, 
                                                 Integer.MAX_VALUE, 
                                                 (path, attr) -> 
                                                 path.toString().endsWith(".txt"))) {
                stream.forEach(System.out::println);
            }
            
            // Limpando
            deletarRecursivamente(diretorio);
            System.out.println("Diretório removido recursivamente");
            
        } catch (IOException e) {
            System.out.println("Erro nas operações de diretório: " + e.getMessage());
        }
    }
    
    private static void deletarRecursivamente(Path path) throws IOException {
        if (Files.isDirectory(path)) {
            try (Stream<Path> entries = Files.list(path)) {
                entries.forEach(entry -> {
                    try {
                        deletarRecursivamente(entry);
                    } catch (IOException e) {
                        throw new UncheckedIOException(e);
                    }
                });
            }
        }
        Files.deleteIfExists(path);
    }
    
    public static void demonstrarFileChannel() {
        System.out.println("\n=== FILECHANNEL ===");
        
        // Escrita com FileChannel
        try (FileChannel channel = FileChannel.open(
             Paths.get("channel_exemplo.txt"), 
             StandardOpenOption.CREATE, 
             StandardOpenOption.WRITE)) {
            
            String texto = "Este é um exemplo de FileChannel!\n";
            texto += "FileChannel oferece operações de I/O mais eficientes.\n";
            texto += "Suporte a scatter/gather e file locking.\n";
            
            ByteBuffer buffer = ByteBuffer.allocate(1024);
            buffer.put(texto.getBytes(StandardCharsets.UTF_8));
            buffer.flip(); // Prepara para leitura
            
            channel.write(buffer);
            System.out.println("Dados escritos com FileChannel");
            
        } catch (IOException e) {
            System.out.println("Erro na escrita com FileChannel: " + e.getMessage());
        }
        
        // Leitura com FileChannel
        try (FileChannel channel = FileChannel.open(
             Paths.get("channel_exemplo.txt"), 
             StandardOpenOption.READ)) {
            
            ByteBuffer buffer = ByteBuffer.allocate(1024);
            StringBuilder conteudo = new StringBuilder();
            
            while (channel.read(buffer) > 0) {
                buffer.flip(); // Prepara para leitura
                while (buffer.hasRemaining()) {
                    conteudo.append((char) buffer.get());
                }
                buffer.clear(); // Prepara para próxima leitura
            }
            
            System.out.println("Conteúdo lido com FileChannel:");
            System.out.println(conteudo.toString());
            
        } catch (IOException e) {
            System.out.println("Erro na leitura com FileChannel: " + e.getMessage());
        }
        
        // File locking
        try (FileChannel channel = FileChannel.open(
             Paths.get("locked_file.txt"), 
             StandardOpenOption.CREATE, 
             StandardOpenOption.WRITE)) {
            
            // Tentativa de lock exclusivo
            FileLock lock = channel.tryLock();
            if (lock != null) {
                System.out.println("Lock adquirido com sucesso!");
                
                // Escrevendo dados
                String dados = "Dados protegidos por lock\n";
                ByteBuffer buffer = ByteBuffer.wrap(dados.getBytes());
                channel.write(buffer);
                
                // Simulando trabalho
                Thread.sleep(2000);
                
                lock.release();
                System.out.println("Lock liberado");
            } else {
                System.out.println("Não foi possível adquirir o lock");
            }
            
        } catch (IOException | InterruptedException e) {
            System.out.println("Erro com file locking: " + e.getMessage());
        }
        
        // Limpeza
        try {
            Files.deleteIfExists(Paths.get("channel_exemplo.txt"));
            Files.deleteIfExists(Paths.get("locked_file.txt"));
        } catch (IOException e) {
            System.out.println("Erro na limpeza: " + e.getMessage());
        }
    }
    
    public static void demonstrarWatchService() {
        System.out.println("\n=== WATCHSERVICE ===");
        
        try {
            Path diretorio = Paths.get("watch_dir");
            Files.createDirectories(diretorio);
            
            WatchService watchService = FileSystems.getDefault().newWatchService();
            diretorio.register(watchService, 
                             StandardWatchEventKinds.ENTRY_CREATE,
                             StandardWatchEventKinds.ENTRY_DELETE,
                             StandardWatchEventKinds.ENTRY_MODIFY);
            
            System.out.println("WatchService iniciado para: " + diretorio);
            System.out.println("Monitorando por 10 segundos...");
            
            // Thread para criar/modificar/deletar arquivos
            Thread modificador = new Thread(() -> {
                try {
                    Thread.sleep(1000);
                    
                    // Criar arquivo
                    Path novoArquivo = diretorio.resolve("teste.txt");
                    Files.writeString(novoArquivo, "Conteúdo inicial");
                    System.out.println("Arquivo criado: " + novoArquivo);
                    
                    Thread.sleep(1000);
                    
                    // Modificar arquivo
                    Files.writeString(novoArquivo, "Conteúdo modificado", 
                                    StandardOpenOption.APPEND);
                    System.out.println("Arquivo modificado: " + novoArquivo);
                    
                    Thread.sleep(1000);
                    
                    // Deletar arquivo
                    Files.delete(novoArquivo);
                    System.out.println("Arquivo deletado: " + novoArquivo);
                    
                } catch (IOException | InterruptedException e) {
                    e.printStackTrace();
                }
            });
            
            modificador.start();
            
            // Monitorando eventos
            long startTime = System.currentTimeMillis();
            while (System.currentTimeMillis() - startTime < 10000) {
                WatchKey key = watchService.poll(1, TimeUnit.SECONDS);
                if (key != null) {
                    for (WatchEvent<?> event : key.pollEvents()) {
                        WatchEvent.Kind<?> kind = event.kind();
                        Path path = (Path) event.context();
                        
                        System.out.printf("Evento: %s - Arquivo: %s%n", kind, path);
                        
                        if (kind == StandardWatchEventKinds.OVERFLOW) {
                            System.out.println("Evento de overflow ocorreu");
                        }
                    }
                    
                    boolean valid = key.reset();
                    if (!valid) {
                        System.out.println("WatchKey não é mais válido");
                        break;
                    }
                }
            }
            
            watchService.close();
            deletarRecursivamente(diretorio);
            System.out.println("WatchService finalizado");
            
        } catch (IOException | InterruptedException e) {
            System.out.println("Erro no WatchService: " + e.getMessage());
        }
    }
}
```

## **12.3 Exercícios Práticos**

### **Exercício 12.1: Utilitário de Backup de Arquivos**

```java
import java.nio.file.*;
import java.nio.file.attribute.BasicFileAttributes;
import java.io.IOException;
import java.util.*;

public class BackupUtility {
    private final Path sourceDir;
    private final Path backupDir;
    
    public BackupUtility(String source, String backup) {
        this.sourceDir = Paths.get(source);
        this.backupDir = Paths.get(backup);
    }
    
    public void createBackup() throws IOException {
        if (!Files.exists(sourceDir)) {
            throw new IOException("Diretório fonte não existe: " + sourceDir);
        }
        
        Files.createDirectories(backupDir);
        
        Files.walkFileTree(sourceDir, new SimpleFileVisitor<Path>() {
            @Override
            public FileVisitResult preVisitDirectory(Path dir, BasicFileAttributes attrs) 
                    throws IOException {
                Path relativePath = sourceDir.relativize(dir);
                Path targetDir = backupDir.resolve(relativePath);
                Files.createDirectories(targetDir);
                return FileVisitResult.CONTINUE;
            }
            
            @Override
            public FileVisitResult visitFile(Path file, BasicFileAttributes attrs) 
                    throws IOException {
                Path relativePath = sourceDir.relativize(file);
                Path targetFile = backupDir.resolve(relativePath);
                
                // Copia apenas se o arquivo foi modificado
                if (!Files.exists(targetFile) || 
                    Files.getLastModifiedTime(file).compareTo(
                    Files.getLastModifiedTime(targetFile)) > 0) {
                    
                    Files.copy(file, targetFile, StandardCopyOption.REPLACE_EXISTING);
                    System.out.println("Backup: " + relativePath);
                }
                
                return FileVisitResult.CONTINUE;
            }
        });
        
        System.out.println("Backup concluído de " + sourceDir + " para " + backupDir);
    }
    
    public static void main(String[] args) {
        if (args.length != 2) {
            System.out.println("Uso: java BackupUtility <diretorio_fonte> <diretorio_backup>");
            return;
        }
        
        BackupUtility backup = new BackupUtility(args[0], args[1]);
        try {
            backup.createBackup();
        } catch (IOException e) {
            System.err.println("Erro no backup: " + e.getMessage());
        }
    }
}
```

### **Exercício 12.2: Analisador de Logs em Tempo Real**

```java
import java.nio.file.*;
import java.nio.charset.StandardCharsets;
import java.io.IOException;
import java.util.*;
import java.util.concurrent.*;

public class LogAnalyzer {
    private final Path logDir;
    private final Map<String, Integer> errorCounts;
    private final ExecutorService executor;
    private volatile boolean running;
    
    public LogAnalyzer(String logDirectory) {
        this.logDir = Paths.get(logDirectory);
        this.errorCounts = new ConcurrentHashMap<>();
        this.executor = Executors.newCachedThreadPool();
        this.running = true;
    }
    
    public void startAnalysis() throws IOException {
        // Analisa arquivos de log existentes
        analyzeExistingLogs();
        
        // Monitora novos arquivos
        startFileWatcher();
    }
    
    private void analyzeExistingLogs() throws IOException {
        if (!Files.exists(logDir)) {
            Files.createDirectories(logDir);
            return;
        }
        
        try (Stream<Path> stream = Files.list(logDir)) {
            stream.filter(path -> path.toString().endsWith(".log"))
                  .forEach(this::analyzeLogFile);
        }
    }
    
    private void startFileWatcher() throws IOException {
        WatchService watchService = FileSystems.getDefault().newWatchService();
        logDir.register(watchService, StandardWatchEventKinds.ENTRY_CREATE);
        
        executor.execute(() -> {
            while (running) {
                try {
                    WatchKey key = watchService.take();
                    for (WatchEvent<?> event : key.pollEvents()) {
                        if (event.kind() == StandardWatchEventKinds.ENTRY_CREATE) {
                            Path newFile = (Path) event.context();
                            if (newFile.toString().endsWith(".log")) {
                                analyzeLogFile(logDir.resolve(newFile));
                            }
                        }
                    }
                    key.reset();
                } catch (InterruptedException e) {
                    break;
                } catch (ClosedWatchServiceException e) {
                    break;
                }
            }
        });
    }
    
    private void analyzeLogFile(Path logFile) {
        executor.execute(() -> {
            try {
                System.out.println("Analisando: " + logFile.getFileName());
                
                List<String> lines = Files.readAllLines(logFile, StandardCharsets.UTF_8);
                for (String line : lines) {
                    if (line.toLowerCase().contains("error")) {
                        String[] parts = line.split(" ");
                        if (parts.length > 0) {
                            String errorType = extractErrorType(line);
                            errorCounts.merge(errorType, 1, Integer::sum);
                        }
                    }
                }
                
                printStatistics();
                
            } catch (IOException e) {
                System.err.println("Erro ao analisar " + logFile + ": " + e.getMessage());
            }
        });
    }
    
    private String extractErrorType(String line) {
        if (line.toLowerCase().contains("nullpointer")) return "NullPointerException";
        if (line.toLowerCase().contains("ioexception")) return "IOException";
        if (line.toLowerCase().contains("timeout")) return "Timeout";
        return "GenericError";
    }
    
    private void printStatistics() {
        System.out.println("\n=== ESTATÍSTICAS DE ERROS ===");
        errorCounts.entrySet().stream()
            .sorted(Map.Entry.<String, Integer>comparingByValue().reversed())
            .forEach(entry -> 
                System.out.printf("%-20s: %d ocorrências%n", entry.getKey(), entry.getValue()));
        System.out.println("=============================\n");
    }
    
    public void stop() {
        running = false;
        executor.shutdown();
        try {
            if (!executor.awaitTermination(5, TimeUnit.SECONDS)) {
                executor.shutdownNow();
            }
        } catch (InterruptedException e) {
            executor.shutdownNow();
        }
    }
    
    public static void main(String[] args) {
        LogAnalyzer analyzer = new LogAnalyzer("logs");
        try {
            analyzer.startAnalysis();
            
            // Executa por 30 segundos
            Thread.sleep(30000);
            analyzer.stop();
            
        } catch (IOException | InterruptedException e) {
            System.err.println("Erro: " + e.getMessage());
            analyzer.stop();
        }
    }
}
```

## **12.4 Questionário de Revisão**

**Questão 1:** Qual a diferença entre InputStream/OutputStream e Reader/Writer?
- A) InputStream/OutputStream trabalham com bytes, Reader/Writer com caracteres
- B) Reader/Writer são mais rápidos para todos os tipos de dados
- C) Não há diferença significativa

**Questão 2:** O que é a classe Files na API NIO.2?
- A) Uma classe utilitária com métodos estáticos para operações em arquivos
- B) Uma substituição completa para a classe File
- C) Uma interface para trabalhar com file systems

**Questão 3:** Para que serve o WatchService?
- A) Monitorar mudanças em diretórios e arquivos
- B) Observar o consumo de memória da aplicação
- C) Controlar o acesso concorrente a arquivos

**Questão 4:** Qual a vantagem do FileChannel sobre FileInputStream/FileOutputStream?
- A) Suporte a operações mais avançadas como scatter/gather e file locking
- B) Melhor performance em todos os cenários
- C) Sintaxe mais simples

**Questão 5:** O que é um Path na API NIO.2?

## **12.5 Laboratório Prático**

**Projeto: Sistema de Gerenciamento de Arquivos**

```java
// Implemente um sistema de gerenciamento de arquivos com:
// 1. Navegação em árvore de diretórios
// 2. Operações CRUD (criar, ler, atualizar, deletar)
// 3. Busca por nome, tipo e conteúdo
// 4. Estatísticas de uso (tamanho, quantidade)
// 5. Backup incremental automático

// Use Files, Path, FileVisitor, e outras classes NIO.2
```

## **12.6 Material de Apoio**

**Hierarquia de I/O:**

**Streams Binárias:**
- `InputStream` / `OutputStream`
- `FileInputStream` / `FileOutputStream`
- `BufferedInputStream` / `BufferedOutputStream`
- `DataInputStream` / `DataOutputStream`

**Streams de Texto:**
- `Reader` / `Writer`
- `FileReader` / `FileWriter`
- `BufferedReader` / `BufferedWriter`
- `InputStreamReader` / `OutputStreamWriter`

**API NIO.2:**
- `Path` - Representação de caminhos
- `Files` - Operações utilitárias
- `Paths` - Fábrica de Paths
- `FileSystems` - Acesso a file systems

**FileChannel:**
- Operações de leitura/escrita eficientes
- File locking
- Memory-mapped files
- Transferência entre channels

**Padrões Comuns:**
- Decorator Pattern (Buffered streams)
- Visitor Pattern (FileVisitor)
- Observer Pattern (WatchService)

**Dicas Importantes:**
- Sempre use try-with-resources com streams
- Prefira NIO.2 sobre java.io.File
- Use BufferedReader/BufferedWriter para texto
- Files.readAllLines() é conveniente para arquivos pequenos
- WatchService é ideal para monitoramento de diretórios
- FileChannel oferece melhor performance para operações grandes

---

**Próximo Módulo: JDBC e Bancos de Dados**

# **Módulo 13: JDBC e Bancos de Dados**

## **13.1 Objetivos do Módulo**

- Compreender a arquitetura do JDBC e seus componentes principais
- Dominar a conexão com bancos de dados relacionais
- Aprender a executar consultas SQL (SELECT, INSERT, UPDATE, DELETE)
- Trabalhar com transações e controle de concorrência
- Implementar padrões de acesso a dados (DAO)
- Conhecer boas práticas de performance e segurança

## **13.2 Conteúdo Programático**

### **13.2.1 Fundamentos do JDBC**

**Exemplo 13.1: Configuração e Conexão Básica**

```java
import java.sql.*;
import java.util.Properties;

public class ExemploJDBCBasico {

    public static void main(String[] args) {
        System.out.println("=== FUNDAMENTOS DO JDBC ===");
        
        // Configuração de conexão
        demonstrarConfiguracao();
        
        // Operações básicas CRUD
        demonstrarCRUD();
        
        // Transações
        demonstrarTransacoes();
        
        // Metadados
        demonstrarMetadados();
    }
    
    public static void demonstrarConfiguracao() {
        System.out.println("\n=== CONFIGURAÇÃO DE CONEXÃO ===");
        
        // URL de conexão para diferentes bancos
        String urlMySQL = "jdbc:mysql://localhost:3306/meubanco";
        String urlPostgreSQL = "jdbc:postgresql://localhost:5432/meubanco";
        String urlH2 = "jdbc:h2:mem:testdb";
        
        Connection conexao = null;
        
        try {
            // Método 1: DriverManager com Properties
            Properties props = new Properties();
            props.setProperty("user", "usuario");
            props.setProperty("password", "senha");
            props.setProperty("useSSL", "false");
            props.setProperty("serverTimezone", "UTC");
            
            // Método 2: DriverManager com parâmetros
            conexao = DriverManager.getConnection(urlH2, "sa", "");
            
            // Verificando se a conexão foi bem sucedida
            if (conexao != null && !conexao.isClosed()) {
                System.out.println("✅ Conexão estabelecida com sucesso!");
                
                // Informações da conexão
                DatabaseMetaData metaData = conexao.getMetaData();
                System.out.println("Database: " + metaData.getDatabaseProductName());
                System.out.println("Versão: " + metaData.getDatabaseProductVersion());
                System.out.println("Driver: " + metaData.getDriverName());
                System.out.println("Versão Driver: " + metaData.getDriverVersion());
                System.out.println("URL: " + metaData.getURL());
                System.out.println("Usuário: " + metaData.getUserName());
                
                // Criando tabela de exemplo
                criarTabelaExemplo(conexao);
            }
            
        } catch (SQLException e) {
            System.err.println("❌ Erro na conexão: " + e.getMessage());
            e.printStackTrace();
        } finally {
            // Fechando conexão
            if (conexao != null) {
                try {
                    conexao.close();
                    System.out.println("Conexão fechada.");
                } catch (SQLException e) {
                    System.err.println("Erro ao fechar conexão: " + e.getMessage());
                }
            }
        }
    }
    
    private static void criarTabelaExemplo(Connection conexao) throws SQLException {
        String sql = """
            CREATE TABLE IF NOT EXISTS clientes (
                id INT AUTO_INCREMENT PRIMARY KEY,
                nome VARCHAR(100) NOT NULL,
                email VARCHAR(100) UNIQUE,
                idade INT,
                salario DECIMAL(10,2),
                data_cadastro TIMESTAMP DEFAULT CURRENT_TIMESTAMP
            )
            """;
        
        try (Statement stmt = conexao.createStatement()) {
            stmt.execute(sql);
            System.out.println("✅ Tabela 'clientes' criada com sucesso!");
        }
    }
    
    public static void demonstrarCRUD() {
        System.out.println("\n=== OPERAÇÕES CRUD ===");
        
        String url = "jdbc:h2:mem:testdb";
        
        try (Connection conexao = DriverManager.getConnection(url, "sa", "")) {
            criarTabelaExemplo(conexao);
            
            // CREATE - Inserir dados
            System.out.println("\n--- INSERT ---");
            inserirClientes(conexao);
            
            // READ - Consultar dados
            System.out.println("\n--- SELECT ---");
            consultarClientes(conexao);
            
            // UPDATE - Atualizar dados
            System.out.println("\n--- UPDATE ---");
            atualizarCliente(conexao);
            
            // DELETE - Remover dados
            System.out.println("\n--- DELETE ---");
            deletarCliente(conexao);
            
            // Consulta final
            System.out.println("\n--- CONSULTA FINAL ---");
            consultarClientes(conexao);
            
        } catch (SQLException e) {
            System.err.println("Erro nas operações CRUD: " + e.getMessage());
        }
    }
    
    private static void inserirClientes(Connection conexao) throws SQLException {
        // Inserção com Statement (NÃO recomendado para dados variáveis)
        String sql1 = """
            INSERT INTO clientes (nome, email, idade, salario) 
            VALUES ('João Silva', 'joao@email.com', 30, 5000.00)
            """;
        
        try (Statement stmt = conexao.createStatement()) {
            int linhasAfetadas = stmt.executeUpdate(sql1);
            System.out.println(linhasAfetadas + " linha(s) inserida(s) com Statement");
        }
        
        // Inserção com PreparedStatement (RECOMENDADO)
        String sql2 = """
            INSERT INTO clientes (nome, email, idade, salario) 
            VALUES (?, ?, ?, ?)
            """;
        
        try (PreparedStatement pstmt = conexao.prepareStatement(sql2)) {
            // Primeiro cliente
            pstmt.setString(1, "Maria Santos");
            pstmt.setString(2, "maria@email.com");
            pstmt.setInt(3, 25);
            pstmt.setDouble(4, 4500.00);
            pstmt.executeUpdate();
            
            // Segundo cliente
            pstmt.setString(1, "Pedro Oliveira");
            pstmt.setString(2, "pedro@email.com");
            pstmt.setInt(3, 35);
            pstmt.setDouble(4, 6000.00);
            pstmt.executeUpdate();
            
            // Terceiro cliente
            pstmt.setString(1, "Ana Costa");
            pstmt.setString(2, "ana@email.com");
            pstmt.setInt(3, 28);
            pstmt.setDouble(4, 5500.00);
            pstmt.executeUpdate();
            
            System.out.println("3 clientes inseridos com PreparedStatement");
        }
        
        // Inserção com batch (para múltiplas inserções)
        String sql3 = "INSERT INTO clientes (nome, email, idade) VALUES (?, ?, ?)";
        
        try (PreparedStatement pstmt = conexao.prepareStatement(sql3)) {
            pstmt.setString(1, "Carlos Souza");
            pstmt.setString(2, "carlos@email.com");
            pstmt.setInt(3, 40);
            pstmt.addBatch();
            
            pstmt.setString(1, "Julia Lima");
            pstmt.setString(2, "julia@email.com");
            pstmt.setInt(3, 22);
            pstmt.addBatch();
            
            int[] resultados = pstmt.executeBatch();
            System.out.println("Batch executado: " + resultados.length + " inserções");
        }
    }
    
    private static void consultarClientes(Connection conexao) throws SQLException {
        // Consulta simples
        String sql1 = "SELECT * FROM clientes";
        
        try (Statement stmt = conexao.createStatement();
             ResultSet rs = stmt.executeQuery(sql1)) {
            
            System.out.println("\nTodos os clientes:");
            while (rs.next()) {
                int id = rs.getInt("id");
                String nome = rs.getString("nome");
                String email = rs.getString("email");
                int idade = rs.getInt("idade");
                double salario = rs.getDouble("salario");
                Date dataCadastro = rs.getDate("data_cadastro");
                
                System.out.printf("ID: %d, Nome: %s, Email: %s, Idade: %d, Salário: %.2f, Cadastro: %s%n",
                                id, nome, email, idade, salario, dataCadastro);
            }
        }
        
        // Consulta com PreparedStatement e filtro
        String sql2 = "SELECT * FROM clientes WHERE idade > ? AND salario >= ?";
        
        try (PreparedStatement pstmt = conexao.prepareStatement(sql2)) {
            pstmt.setInt(1, 25);
            pstmt.setDouble(2, 5000.00);
            
            try (ResultSet rs = pstmt.executeQuery()) {
                System.out.println("\nClientes com idade > 25 e salário >= 5000:");
                while (rs.next()) {
                    System.out.printf("ID: %d, Nome: %s, Idade: %d, Salário: %.2f%n",
                                    rs.getInt("id"), rs.getString("nome"),
                                    rs.getInt("idade"), rs.getDouble("salario"));
                }
            }
        }
        
        // Consulta com ordenação e limite
        String sql3 = "SELECT nome, salario FROM clientes ORDER BY salario DESC LIMIT 3";
        
        try (Statement stmt = conexao.createStatement();
             ResultSet rs = stmt.executeQuery(sql3)) {
            
            System.out.println("\nTop 3 clientes por salário:");
            while (rs.next()) {
                System.out.printf("Nome: %s, Salário: %.2f%n",
                                rs.getString("nome"), rs.getDouble("salario"));
            }
        }
    }
    
    private static void atualizarCliente(Connection conexao) throws SQLException {
        String sql = "UPDATE clientes SET salario = salario * 1.1 WHERE idade > ?";
        
        try (PreparedStatement pstmt = conexao.prepareStatement(sql)) {
            pstmt.setInt(1, 30);
            
            int linhasAfetadas = pstmt.executeUpdate();
            System.out.println(linhasAfetadas + " cliente(s) tiveram aumento de 10%");
        }
        
        // Atualização específica
        String sql2 = "UPDATE clientes SET email = ? WHERE nome = ?";
        
        try (PreparedStatement pstmt = conexao.prepareStatement(sql2)) {
            pstmt.setString(1, "joao.novo@email.com");
            pstmt.setString(2, "João Silva");
            
            int linhasAfetadas = pstmt.executeUpdate();
            if (linhasAfetadas > 0) {
                System.out.println("Email do João atualizado");
            }
        }
    }
    
    private static void deletarCliente(Connection conexao) throws SQLException {
        String sql = "DELETE FROM clientes WHERE idade < ?";
        
        try (PreparedStatement pstmt = conexao.ppareStatement(sql)) {
            pstmt.setInt(1, 25);
            
            int linhasAfetadas = pstmt.executeUpdate();
            System.out.println(linhasAfetadas + " cliente(s) menores de 25 anos removidos");
        }
    }
    
    public static void demonstrarTransacoes() {
        System.out.println("\n=== CONTROLE DE TRANSAÇÕES ===");
        
        String url = "jdbc:h2:mem:testdb";
        Connection conexao = null;
        
        try {
            conexao = DriverManager.getConnection(url, "sa", "");
            criarTabelaExemplo(conexao);
            
            // Desativar auto-commit para controle manual
            conexao.setAutoCommit(false);
            System.out.println("Auto-commit desativado");
            
            try {
                // Operação 1 - Inserir cliente
                String sql1 = "INSERT INTO clientes (nome, email, idade, salario) VALUES (?, ?, ?, ?)";
                try (PreparedStatement pstmt = conexao.prepareStatement(sql1)) {
                    pstmt.setString(1, "Carlos Transacao");
                    pstmt.setString(2, "carlos.t@email.com");
                    pstmt.setInt(3, 45);
                    pstmt.setDouble(4, 8000.00);
                    pstmt.executeUpdate();
                    System.out.println("Operação 1: Cliente Carlos inserido");
                }
                
                // Operação 2 - Atualizar salários
                String sql2 = "UPDATE clientes SET salario = salario * 1.05 WHERE salario < ?";
                try (PreparedStatement pstmt = conexao.prepareStatement(sql2)) {
                    pstmt.setDouble(1, 6000.00);
                    int linhas = pstmt.executeUpdate();
                    System.out.println("Operação 2: " + linhas + " salários atualizados");
                }
                
                // Simular um erro para testar rollback
                boolean simularErro = false; // Altere para true para testar rollback
                if (simularErro) {
                    throw new SQLException("Erro simulado para teste de rollback");
                }
                
                // Commit das operações
                conexao.commit();
                System.out.println("✅ Transação commitada com sucesso!");
                
            } catch (SQLException e) {
                // Rollback em caso de erro
                conexao.rollback();
                System.out.println("❌ Erro na transação. Rollback executado: " + e.getMessage());
            }
            
            // Verificar resultado
            consultarClientes(conexao);
            
        } catch (SQLException e) {
            System.err.println("Erro no controle de transações: " + e.getMessage());
        } finally {
            if (conexao != null) {
                try {
                    // Restaurar auto-commit
                    conexao.setAutoCommit(true);
                    conexao.close();
                } catch (SQLException e) {
                    System.err.println("Erro ao fechar conexão: " + e.getMessage());
                }
            }
        }
    }
    
    public static void demonstrarMetadados() {
        System.out.println("\n=== METADADOS DO BANCO ===");
        
        String url = "jdbc:h2:mem:testdb";
        
        try (Connection conexao = DriverManager.getConnection(url, "sa", "")) {
            
            // Metadados do banco
            DatabaseMetaData dbMetaData = conexao.getMetaData();
            
            System.out.println("=== METADADOS DO BANCO ===");
            System.out.println("Produto: " + dbMetaData.getDatabaseProductName());
            System.out.println("Versão: " + dbMetaData.getDatabaseProductVersion());
            System.out.println("Driver: " + dbMetaData.getDriverName());
            System.out.println("Versão Driver: " + dbMetaData.getDriverVersion());
            System.out.println("URL: " + dbMetaData.getURL());
            System.out.println("Usuário: " + dbMetaData.getUserName());
            
            System.out.println("\n=== RECURSOS SUPORTADOS ===");
            System.out.println("Suporta transações: " + dbMetaData.supportsTransactions());
            System.out.println("Suporta batch updates: " + dbMetaData.supportsBatchUpdates());
            System.out.println("Suporta ResultSet.TYPE_SCROLL_INSENSITIVE: " + 
                             dbMetaData.supportsResultSetType(ResultSet.TYPE_SCROLL_INSENSITIVE));
            
            // Metadados das tabelas
            System.out.println("\n=== TABELAS DO BANCO ===");
            try (ResultSet tabelas = dbMetaData.getTables(null, null, "%", new String[]{"TABLE"})) {
                while (tabelas.next()) {
                    String nomeTabela = tabelas.getString("TABLE_NAME");
                    String tipo = tabelas.getString("TABLE_TYPE");
                    System.out.println("Tabela: " + nomeTabela + " (" + tipo + ")");
                    
                    // Metadados das colunas
                    try (ResultSet colunas = dbMetaData.getColumns(null, null, nomeTabela, "%")) {
                        while (colunas.next()) {
                            String nomeColuna = colunas.getString("COLUMN_NAME");
                            String tipoColuna = colunas.getString("TYPE_NAME");
                            int tamanho = colunas.getInt("COLUMN_SIZE");
                            System.out.println("  Coluna: " + nomeColuna + " (" + tipoColuna + "(" + tamanho + "))");
                        }
                    }
                }
            }
            
            // Metadados de um ResultSet
            System.out.println("\n=== METADADOS DO RESULTSET ===");
            String sql = "SELECT id, nome, email, idade, salario FROM clientes";
            try (Statement stmt = conexao.createStatement();
                 ResultSet rs = stmt.executeQuery(sql)) {
                
                ResultSetMetaData rsMetaData = rs.getMetaData();
                int colunaCount = rsMetaData.getColumnCount();
                
                System.out.println("Número de colunas: " + colunaCount);
                for (int i = 1; i <= colunaCount; i++) {
                    System.out.printf("Coluna %d: %s (%s)%n", 
                                    i, 
                                    rsMetaData.getColumnName(i),
                                    rsMetaData.getColumnTypeName(i));
                }
            }
            
        } catch (SQLException e) {
            System.err.println("Erro ao recuperar metadados: " + e.getMessage());
        }
    }
}
```

### **13.2.2 Padrão DAO (Data Access Object)**

**Exemplo 13.2: Implementação do Padrão DAO**

```java
import java.sql.*;
import java.util.*;
import java.util.Date;

// Interface do DAO
interface ClienteDAO {
    void inserir(Cliente cliente) throws SQLException;
    Optional<Cliente> buscarPorId(int id) throws SQLException;
    List<Cliente> listarTodos() throws SQLException;
    void atualizar(Cliente cliente) throws SQLException;
    void deletar(int id) throws SQLException;
    List<Cliente> buscarPorNome(String nome) throws SQLException;
}

// Classe de entidade
class Cliente {
    private Integer id;
    private String nome;
    private String email;
    private Integer idade;
    private Double salario;
    private Date dataCadastro;
    
    // Construtores
    public Cliente() {}
    
    public Cliente(String nome, String email, Integer idade, Double salario) {
        this.nome = nome;
        this.email = email;
        this.idade = idade;
        this.salario = salario;
    }
    
    // Getters e Setters
    public Integer getId() { return id; }
    public void setId(Integer id) { this.id = id; }
    
    public String getNome() { return nome; }
    public void setNome(String nome) { this.nome = nome; }
    
    public String getEmail() { return email; }
    public void setEmail(String email) { this.email = email; }
    
    public Integer getIdade() { return idade; }
    public void setIdade(Integer idade) { this.idade = idade; }
    
    public Double getSalario() { return salario; }
    public void setSalario(Double salario) { this.salario = salario; }
    
    public Date getDataCadastro() { return dataCadastro; }
    public void setDataCadastro(Date dataCadastro) { this.dataCadastro = dataCadastro; }
    
    @Override
    public String toString() {
        return String.format("Cliente{id=%d, nome='%s', email='%s', idade=%d, salario=%.2f}",
                           id, nome, email, idade, salario);
    }
}

// Implementação concreta do DAO
class ClienteDAOImpl implements ClienteDAO {
    private final ConnectionFactory connectionFactory;
    
    public ClienteDAOImpl(ConnectionFactory connectionFactory) {
        this.connectionFactory = connectionFactory;
        criarTabelaSeNecessario();
    }
    
    private void criarTabelaSeNecessario() {
        String sql = """
            CREATE TABLE IF NOT EXISTS clientes (
                id INT AUTO_INCREMENT PRIMARY KEY,
                nome VARCHAR(100) NOT NULL,
                email VARCHAR(100) UNIQUE,
                idade INT,
                salario DECIMAL(10,2),
                data_cadastro TIMESTAMP DEFAULT CURRENT_TIMESTAMP
            )
            """;
        
        try (Connection conexao = connectionFactory.getConnection();
             Statement stmt = conexao.createStatement()) {
            stmt.execute(sql);
        } catch (SQLException e) {
            throw new RuntimeException("Erro ao criar tabela", e);
        }
    }
    
    @Override
    public void inserir(Cliente cliente) throws SQLException {
        String sql = """
            INSERT INTO clientes (nome, email, idade, salario) 
            VALUES (?, ?, ?, ?)
            """;
        
        try (Connection conexao = connectionFactory.getConnection();
             PreparedStatement pstmt = conexao.prepareStatement(sql, Statement.RETURN_GENERATED_KEYS)) {
            
            pstmt.setString(1, cliente.getNome());
            pstmt.setString(2, cliente.getEmail());
            
            if (cliente.getIdade() != null) {
                pstmt.setInt(3, cliente.getIdade());
            } else {
                pstmt.setNull(3, Types.INTEGER);
            }
            
            if (cliente.getSalario() != null) {
                pstmt.setDouble(4, cliente.getSalario());
            } else {
                pstmt.setNull(4, Types.DECIMAL);
            }
            
            int linhasAfetadas = pstmt.executeUpdate();
            
            if (linhasAfetadas > 0) {
                try (ResultSet generatedKeys = pstmt.getGeneratedKeys()) {
                    if (generatedKeys.next()) {
                        cliente.setId(generatedKeys.getInt(1));
                    }
                }
            }
        }
    }
    
    @Override
    public Optional<Cliente> buscarPorId(int id) throws SQLException {
        String sql = "SELECT * FROM clientes WHERE id = ?";
        
        try (Connection conexao = connectionFactory.getConnection();
             PreparedStatement pstmt = conexao.prepareStatement(sql)) {
            
            pstmt.setInt(1, id);
            
            try (ResultSet rs = pstmt.executeQuery()) {
                if (rs.next()) {
                    return Optional.of(mapearResultSetParaCliente(rs));
                } else {
                    return Optional.empty();
                }
            }
        }
    }
    
    @Override
    public List<Cliente> listarTodos() throws SQLException {
        String sql = "SELECT * FROM clientes ORDER BY nome";
        List<Cliente> clientes = new ArrayList<>();
        
        try (Connection conexao = connectionFactory.getConnection();
             Statement stmt = conexao.createStatement();
             ResultSet rs = stmt.executeQuery(sql)) {
            
            while (rs.next()) {
                clientes.add(mapearResultSetParaCliente(rs));
            }
        }
        
        return clientes;
    }
    
    @Override
    public void atualizar(Cliente cliente) throws SQLException {
        String sql = """
            UPDATE clientes 
            SET nome = ?, email = ?, idade = ?, salario = ? 
            WHERE id = ?
            """;
        
        try (Connection conexao = connectionFactory.getConnection();
             PreparedStatement pstmt = conexao.prepareStatement(sql)) {
            
            pstmt.setString(1, cliente.getNome());
            pstmt.setString(2, cliente.getEmail());
            
            if (cliente.getIdade() != null) {
                pstmt.setInt(3, cliente.getIdade());
            } else {
                pstmt.setNull(3, Types.INTEGER);
            }
            
            if (cliente.getSalario() != null) {
                pstmt.setDouble(4, cliente.getSalario());
            } else {
                pstmt.setNull(4, Types.DECIMAL);
            }
            
            pstmt.setInt(5, cliente.getId());
            
            pstmt.executeUpdate();
        }
    }
    
    @Override
    public void deletar(int id) throws SQLException {
        String sql = "DELETE FROM clientes WHERE id = ?";
        
        try (Connection conexao = connectionFactory.getConnection();
             PreparedStatement pstmt = conexao.prepareStatement(sql)) {
            
            pstmt.setInt(1, id);
            pstmt.executeUpdate();
        }
    }
    
    @Override
    public List<Cliente> buscarPorNome(String nome) throws SQLException {
        String sql = "SELECT * FROM clientes WHERE nome LIKE ? ORDER BY nome";
        List<Cliente> clientes = new ArrayList<>();
        
        try (Connection conexao = connectionFactory.getConnection();
             PreparedStatement pstmt = conexao.prepareStatement(sql)) {
            
            pstmt.setString(1, "%" + nome + "%");
            
            try (ResultSet rs = pstmt.executeQuery()) {
                while (rs.next()) {
                    clientes.add(mapearResultSetParaCliente(rs));
                }
            }
        }
        
        return clientes;
    }
    
    private Cliente mapearResultSetParaCliente(ResultSet rs) throws SQLException {
        Cliente cliente = new Cliente();
        cliente.setId(rs.getInt("id"));
        cliente.setNome(rs.getString("nome"));
        cliente.setEmail(rs.getString("email"));
        cliente.setIdade(rs.getInt("idade"));
        if (rs.wasNull()) cliente.setIdade(null);
        cliente.setSalario(rs.getDouble("salario"));
        if (rs.wasNull()) cliente.setSalario(null);
        cliente.setDataCadastro(rs.getDate("data_cadastro"));
        return cliente;
    }
}

// Factory para conexões
class ConnectionFactory {
    private final String url;
    private final String usuario;
    private final String senha;
    
    public ConnectionFactory(String url, String usuario, String senha) {
        this.url = url;
        this.usuario = usuario;
        this.senha = senha;
    }
    
    public Connection getConnection() throws SQLException {
        return DriverManager.getConnection(url, usuario, senha);
    }
}

// Classe de teste do DAO
public class ExemploPadraoDAO {
    public static void main(String[] args) {
        System.out.println("=== PADRÃO DAO ===");
        
        // Configuração
        String url = "jdbc:h2:mem:testdb";
        ConnectionFactory connectionFactory = new ConnectionFactory(url, "sa", "");
        ClienteDAO clienteDAO = new ClienteDAOImpl(connectionFactory);
        
        try {
            // Teste das operações
            testarOperacoesDAO(clienteDAO);
            
        } catch (SQLException e) {
            System.err.println("Erro nas operações DAO: " + e.getMessage());
            e.printStackTrace();
        }
    }
    
    private static void testarOperacoesDAO(ClienteDAO clienteDAO) throws SQLException {
        // Inserir clientes
        System.out.println("\n--- INSERINDO CLIENTES ---");
        Cliente cliente1 = new Cliente("Ana Silva", "ana.silva@email.com", 28, 5500.00);
        Cliente cliente2 = new Cliente("Carlos Oliveira", "carlos.oliveira@email.com", 35, 7200.00);
        Cliente cliente3 = new Cliente("Beatriz Costa", "beatriz.costa@email.com", null, 4800.00);
        
        clienteDAO.inserir(cliente1);
        clienteDAO.inserir(cliente2);
        clienteDAO.inserir(cliente3);
        
        System.out.println("Clientes inseridos com IDs: " + 
                          cliente1.getId() + ", " + cliente2.getId() + ", " + cliente3.getId());
        
        // Listar todos
        System.out.println("\n--- LISTANDO TODOS OS CLIENTES ---");
        List<Cliente> todosClientes = clienteDAO.listarTodos();
        todosClientes.forEach(System.out::println);
        
        // Buscar por ID
        System.out.println("\n--- BUSCANDO POR ID ---");
        Optional<Cliente> clienteEncontrado = clienteDAO.buscarPorId(cliente1.getId());
        clienteEncontrado.ifPresentOrElse(
            cliente -> System.out.println("Cliente encontrado: " + cliente),
            () -> System.out.println("Cliente não encontrado")
        );
        
        // Buscar por nome
        System.out.println("\n--- BUSCANDO POR NOME ---");
        List<Cliente> clientesComA = clienteDAO.buscarPorNome("a");
        System.out.println("Clientes com 'a' no nome:");
        clientesComA.forEach(System.out::println);
        
        // Atualizar cliente
        System.out.println("\n--- ATUALIZANDO CLIENTE ---");
        cliente1.setSalario(6000.00);
        cliente1.setEmail("ana.silva.novo@email.com");
        clienteDAO.atualizar(cliente1);
        
        clienteDAO.buscarPorId(cliente1.getId())
                 .ifPresent(c -> System.out.println("Cliente atualizado: " + c));
        
        // Deletar cliente
        System.out.println("\n--- DELETANDO CLIENTE ---");
        clienteDAO.deletar(cliente3.getId());
        System.out.println("Cliente com ID " + cliente3.getId() + " deletado");
        
        // Lista final
        System.out.println("\n--- LISTA FINAL ---");
        clienteDAO.listarTodos().forEach(System.out::println);
    }
}
```

## **13.3 Exercícios Práticos**

### **Exercício 13.1: Sistema de Gerenciamento de Produtos**

```java
// Implemente um sistema completo de gerenciamento de produtos com:
// 1. Cadastro de produtos (nome, descrição, preço, quantidade)
// 2. Atualização de estoque
// 3. Busca por nome e faixa de preço
// 4. Relatórios de produtos mais vendidos
// 5. Controle de transações para operações de estoque

// Use o padrão DAO e PreparedStatement para todas as operações
```

### **Exercício 13.2: Sistema de Vendas com Transações**

```java
// Implemente um sistema de vendas que:
// 1. Registra vendas com múltiplos itens
// 2. Atualiza estoque atomicamente
// 3. Usa transações para garantir consistência
// 4. Gera relatórios de vendas por período
// 5. Implementa rollback em caso de erro

// Use transações JDBC e tratamento adequado de exceções
```

## **13.4 Questionário de Revisão**

**Questão 1:** Qual a vantagem do PreparedStatement sobre o Statement?
- A) Prevenção de SQL Injection e melhor performance
- B) Sintaxe mais simples
- C) Suporte a todos os tipos de bancos de dados

**Questão 2:** Quando devemos usar transações em JDBC?
- A) Quando múltiplas operações devem ser atomicas
- B) Sempre que usamos SELECT
- C) Apenas em operações de DELETE

**Questão 3:** O que é o padrão DAO?
- A) Padrão que separa a lógica de acesso a dados da lógica de negócio
- B) Um tipo de banco de dados
- C) Um framework para JDBC

**Questão 4:** Para que serve o método `executeBatch()`?
- A) Executar múltiplas operações em lote
- B) Executar stored procedures
- C) Fazer backup do banco

**Questão 5:** Como previnir SQL Injection em JDBC?

## **13.5 Laboratório Prático**

**Projeto: Sistema Bancário com JDBC**

```java
// Implemente um sistema bancário completo com:
// 1. Cadastro de clientes e contas
// 2. Operações de depósito, saque e transferência
// 3. Extrato por período
// 4. Controle de transações para operações financeiras
// 5. Relatórios de movimentação

// Use transações, DAO pattern e tratamento robusto de erros
```

## **13.6 Material de Apoio**

**Componentes Principais do JDBC:**

**Drivers:**
- Tipo 1: JDBC-ODBC Bridge
- Tipo 2: Native-API/partly Java driver
- Tipo 3: Network Protocol/all-Java driver
- Tipo 4: Native Protocol/all-Java driver (mais comum)

**Interfaces Principais:**
- `DriverManager`: Gerencia drivers e conexões
- `Connection`: Representa conexão com o banco
- `Statement`: Executa queries estáticas
- `PreparedStatement`: Executa queries parametrizadas
- `CallableStatement`: Executa stored procedures
- `ResultSet`: Representa resultados de queries

**Tipos de ResultSet:**
- `TYPE_FORWARD_ONLY`: Só avança (padrão)
- `TYPE_SCROLL_INSENSITIVE`: Navegação bidirecional, insensível a mudanças
- `TYPE_SCROLL_SENSITIVE`: Navegação bidirecional, sensível a mudanças

**Níveis de Concorrência:**
- `CONCUR_READ_ONLY`: Apenas leitura (padrão)
- `CONCUR_UPDATABLE`: Permite atualizações

**Boas Práticas:**
- Sempre use try-with-resources
- Prefira PreparedStatement sobre Statement
- Use conexão pool em produção
- Controle transações explicitamente
- Trate SQLException adequadamente
- Use batch para múltiplas inserções
- Feche recursos na ordem inversa da criação

**Padrões Comuns:**
- DAO (Data Access Object)
- Repository Pattern
- Connection Factory
- Template Method (para operações comuns)

**Dicas de Performance:**
- Use batch operations para múltiplas inserções
- Configure fetch size adequado
- Use connection pooling
- Feche ResultSet, Statement e Connection
- Use índices no banco para queries frequentes

---

**Próximo Módulo: Desenvolvimento Web com Java**

---

# **Módulo 14: Desenvolvimento Web com Java**

## **14.1 Objetivos do Módulo**

- Compreender a arquitetura de aplicações web Java
- Dominar os conceitos de Servlets e JSP
- Aprender padrões de projeto web (MVC)
- Conhecer os fundamentos de APIs REST com JAX-RS
- Entender conceitos de sessão, cookies e segurança web

## **14.2 Conteúdo Programático**

### **14.2.1 Fundamentos de Aplicações Web**

**Exemplo 14.1: Conceitos Básicos de HTTP e Web**

```java
import java.io.*;
import java.net.*;
import java.util.*;

public class FundamentosWeb {

    // Simulação básica de requisição HTTP
    public static void simularRequisicaoHTTP() {
        System.out.println("=== CONCEITOS BÁSICOS DE HTTP ===");

        // Métodos HTTP
        String[] metodos = {"GET", "POST", "PUT", "DELETE", "PATCH", "HEAD", "OPTIONS"};
        System.out.println("Métodos HTTP: " + Arrays.toString(metodos));

        // Códigos de status HTTP
        Map<Integer, String> statusCodes = new HashMap<>();
        statusCodes.put(200, "OK");
        statusCodes.put(201, "Created");
        statusCodes.put(400, "Bad Request");
        statusCodes.put(401, "Unauthorized");
        statusCodes.put(404, "Not Found");
        statusCodes.put(500, "Internal Server Error");

        System.out.println("\nCódigos de Status HTTP:");
        statusCodes.forEach((code, desc) ->
            System.out.println(" " + code + ": " + desc));

        // Headers HTTP comuns
        String[] headers = {
            "Content-Type", "Authorization", "Cookie", "Set-Cookie",
            "Cache-Control", "User-Agent", "Accept", "Content-Length"
        };
        System.out.println("\nHeaders HTTP comuns: " + Arrays.toString(headers));
    }

    // Exemplo de cliente HTTP básico
    public static void clienteHTTPBasico() {
        System.out.println("\n=== CLIENTE HTTP BÁSICO ===");

        try {
            URL url = new URL("https://httpbin.org/get");
            HttpURLConnection conexao = (HttpURLConnection) url.openConnection();

            // Configurar a requisição
            conexao.setRequestMethod("GET");
            conexao.setRequestProperty("User-Agent", "Java-HTTP-Client");
            conexao.setConnectTimeout(5000);
            conexao.setReadTimeout(5000);

            // Ler a resposta
            int statusCode = conexao.getResponseCode();
            System.out.println("Status Code: " + statusCode);

            if (statusCode == 200) {
                BufferedReader reader = new BufferedReader(
                    new InputStreamReader(conexao.getInputStream()));

                String linha;
                StringBuilder resposta = new StringBuilder();
                while ((linha = reader.readLine()) != null) {
                    resposta.append(linha);
                }
                reader.close();

                System.out.println("Resposta: " + resposta.toString().substring(0, 100) + "...");
            }

            conexao.disconnect();

        } catch (IOException e) {
            System.out.println("Erro na requisição: " + e.getMessage());
        }
    }

    // Estrutura de uma aplicação web Java
    public static void estruturaAplicacaoWeb() {
        System.out.println("\n=== ESTRUTURA DE APLICAÇÃO WEB JAVA ===");

        String estrutura = """
            Aplicação Web Java (WAR)
            ├── WEB-INF/
            │   ├── web.xml (Deployment Descriptor)
            │   ├── classes/ (Java Classes)
            │   └── lib/ (JAR dependencies)
            ├── META-INF/
            ├── páginas JSP
            ├── arquivos estáticos (HTML, CSS, JS)
            └── recursos (imagens, etc.)
            """;

        System.out.println(estrutura);

        // Ciclo de vida de uma requisição
        System.out.println("\nCiclo de Vida da Requisição:");
        String cicloVida = """
            1. Cliente envia requisição HTTP
            2. Container Web (Tomcat/Jetty) recebe a requisição
            3. Mapeamento para Servlet/JSP apropriado
            4. Processamento da requisição
            5. Geração da resposta
            6. Envio da resposta ao cliente
            """;
        System.out.println(cicloVida);
    }

    public static void main(String[] args) {
        simularRequisicaoHTTP();
        clienteHTTPBasico();
        estruturaAplicacaoWeb();
    }
}
```

### **14.2.2 Servlets - Fundamentos**

**Exemplo 14.2: Criando e Configurando Servlets**

```java
import javax.servlet.*;
import javax.servlet.http.*;
import javax.servlet.annotation.*;
import java.io.*;
import java.util.*;

// Servlet com anotação (Servlet 3.0+)
@WebServlet(
    name = "ExemploServlet",
    urlPatterns = {"/exemplo", "/demo"},
    loadOnStartup = 1
)
public class ExemploServlet extends HttpServlet {

    private int contadorAcesso;

    @Override
    public void init() throws ServletException {
        contadorAcesso = 0;
        System.out.println("Servlet inicializado: " + getServletName());
    }

    @Override
    protected void doGet(HttpServletRequest request, HttpServletResponse response)
        throws ServletException, IOException {

        contadorAcesso++;

        // Configurar resposta
        response.setContentType("text/html; charset=UTF-8");
        response.setCharacterEncoding("UTF-8");

        // Obter parâmetros da requisição
        String nome = request.getParameter("nome");
        String acao = request.getParameter("acao");

        // Escrever resposta
        PrintWriter out = response.getWriter();
        out.println("<!DOCTYPE html>");
        out.println("<html>");
        out.println("<head>");
        out.println("<title>Exemplo Servlet</title>");
        out.println("<style>");
        out.println("body { font-family: Arial, sans-serif; margin: 40px; }");
        out.println(".info { background: #f0f0f0; padding: 20px; border-radius: 5px; }");
        out.println("</style>");
        out.println("</head>");
        out.println("<body>");
        out.println("<h1>Servlet em Ação!</h1>");

        out.println("<div class='info'>");
        out.println("<h2>Informações da Requisição:</h2>");
        out.println("<p><strong>Método:</strong> " + request.getMethod() + "</p>");
        out.println("<p><strong>URL:</strong> " + request.getRequestURL() + "</p>");
        out.println("<p><strong>Query String:</strong> " + request.getQueryString() + "</p>");
        out.println("<p><strong>Remote Address:</strong> " + request.getRemoteAddr() + "</p>");
        out.println("<p><strong>Contador de Acessos:</strong> " + contadorAcesso + "</p>");

        if (nome != null && !nome.trim().isEmpty()) {
            out.println("<p><strong>Olá:</strong> " + nome + "!</p>");
        }

        if ("redirect".equals(acao)) {
            response.sendRedirect("https://www.google.com");
            return;
        }

        out.println("</div>");

        // Formulário de exemplo
        out.println("<h2>Formulário de Teste</h2>");
        out.println("<form method='post'>");
        out.println("<label for='nome'>Nome:</label>");
        out.println("<input type='text' id='nome' name='nome' required>");
        out.println("<br><br>");
        out.println("<button type='submit'>Enviar via POST</button>");
        out.println("</form>");

        out.println("</body>");
        out.println("</html>");
    }

    @Override
    protected void doPost(HttpServletRequest request, HttpServletResponse response)
        throws ServletException, IOException {

        // Processar dados do formulário
        String nome = request.getParameter("nome");

        // Configurar resposta
        response.setContentType("text/html; charset=UTF-8");

        PrintWriter out = response.getWriter();
        out.println("<!DOCTYPE html>");
        out.println("<html>");
        out.println("<head><title>Resposta POST</title></head>");
        out.println("<body>");
        out.println("<h1>Dados Recebidos!</h1>");
        out.println("<p>Nome recebido: <strong>" + nome + "</strong></p>");
        out.println("<a href='exemplo'>Voltar</a>");
        out.println("</body>");
        out.println("</html>");
    }

    @Override
    public void destroy() {
        System.out.println("Servlet destruído: " + getServletName());
    }
}

// Servlet com manipulação de sessão
@WebServlet("/sessao")
class ServletSessao extends HttpServlet {

    @Override
    protected void doGet(HttpServletRequest request, HttpServletResponse response)
        throws ServletException, IOException {

        response.setContentType("text/html; charset=UTF-8");

        // Obter ou criar sessão
        HttpSession sessao = request.getSession(true);

        // Contador de visitas na sessão
        Integer contadorVisitas = (Integer) sessao.getAttribute("contadorVisitas");
        if (contadorVisitas == null) {
            contadorVisitas = 1;
        } else {
            contadorVisitas++;
        }
        sessao.setAttribute("contadorVisitas", contadorVisitas);

        // Informações da sessão
        String idSessao = sessao.getId();
        long criacao = sessao.getCreationTime();
        long ultimoAcesso = sessao.getLastAccessedTime();
        int maxInativo = sessao.getMaxInactiveInterval();

        PrintWriter out = response.getWriter();
        out.println("<!DOCTYPE html>");
        out.println("<html>");
        out.println("<head><title>Gerenciamento de Sessão</title></head>");
        out.println("<body>");
        out.println("<h1>Informações da Sessão</h1>");
        out.println("<p><strong>ID da Sessão:</strong> " + idSessao + "</p>");
        out.println("<p><strong>Contador de Visitas:</strong> " + contadorVisitas + "</p>");
        out.println("<p><strong>Sessão Criada:</strong> " + new Date(criacao) + "</p>");
        out.println("<p><strong>Último Acesso:</strong> " + new Date(ultimoAcesso) + "</p>");
        out.println("<p><strong>Tempo Máximo Inativo:</strong> " + maxInativo + " segundos</p>");

        // Formulário para invalidar sessão
        out.println("<form method='post'>");
        out.println("<button type='submit' name='acao' value='invalidar'>Invalidar Sessão</button>");
        out.println("</form>");

        out.println("</body>");
        out.println("</html>");
    }

    @Override
    protected void doPost(HttpServletRequest request, HttpServletResponse response)
        throws ServletException, IOException {

        String acao = request.getParameter("acao");

        if ("invalidar".equals(acao)) {
            HttpSession sessao = request.getSession(false);
            if (sessao != null) {
                sessao.invalidate();
            }
            response.sendRedirect("sessao");
        }
    }
}
```

### **14.2.3 JSP (JavaServer Pages)**

**Exemplo 14.3: Páginas JSP e JSTL**

```jsp
<%-- paginaInicial.jsp --%>
<%@ page contentType="text/html;charset=UTF-8" language="java" %>
<%@ taglib prefix="c" uri="http://java.sun.com/jsp/jstl/core" %>
<%@ taglib prefix="fmt" uri="http://java.sun.com/jsp/jstl/fmt" %>
<!DOCTYPE html>
<html>
<head>
    <title>Sistema Web - Página Inicial</title>
    <style>
        body { font-family: Arial, sans-serif; margin: 0; padding: 20px; background: #f5f5f5; }
        .container { max-width: 800px; margin: 0 auto; background: white; padding: 20px; border-radius: 8px; box-shadow: 0 2px 10px rgba(0,0,0,0.1); }
        .header { background: #2c3e50; color: white; padding: 20px; border-radius: 5px; margin-bottom: 20px; }
        .menu { background: #34495e; padding: 10px; border-radius: 5px; margin-bottom: 20px; }
        .menu a { color: white; text-decoration: none; margin-right: 15px; }
        .info-box { background: #ecf0f1; padding: 15px; border-radius: 5px; margin-bottom: 15px; }
        .user-list { width: 100%; border-collapse: collapse; }
        .user-list th, .user-list td { border: 1px solid #bdc3c7; padding: 8px; text-align: left; }
        .user-list th { background: #34495e; color: white; }
    </style>
</head>
<body>
    <div class="container">
        <div class="header">
            <h1>🏢 Sistema de Gerenciamento</h1>
            <p>Bem-vindo ao nosso sistema web desenvolvido em Java</p>
        </div>

        <div class="menu">
            <a href="paginaInicial.jsp">Início</a>
            <a href="usuarios.jsp">Usuários</a>
            <a href="produtos.jsp">Produtos</a>
            <a href="relatorios.jsp">Relatórios</a>
        </div>

        <div class="info-box">
            <h2>📊 Informações do Sistema</h2>

            <%-- Scriptlet JSP (evitar usar em produção) --%>
            <%
                String servidor = request.getServerName();
                int porta = request.getServerPort();
                String contexto = request.getContextPath();
            %>

            <p><strong>Servidor:</strong> <%= servidor %>:<%= porta %></p>
            <p><strong>Contexto:</strong> <%= contexto %></p>
            <p><strong>Data/Hora:</strong> <%= new java.util.Date() %></p>
            <p><strong>User Agent:</strong> ${header['User-Agent']}</p>
        </div>

        <%-- Usando JSTL --%>
        <c:set var="tituloSecao" value="👥 Lista de Usuários" />

        <div class="info-box">
            <h2>${tituloSecao}</h2>

            <c:choose>
                <c:when test="${not empty usuarios}">
                    <table class="user-list">
                        <thead>
                            <tr>
                                <th>ID</th>
                                <th>Nome</th>
                                <th>Email</th>
                                <th>Idade</th>
                                <th>Status</th>
                            </tr>
                        </thead>
                        <tbody>
                            <c:forEach var="usuario" items="${usuarios}" varStatus="status">
                                <tr>
                                    <td>${usuario.id}</td>
                                    <td>${usuario.nome}</td>
                                    <td>${usuario.email}</td>
                                    <td>${usuario.idade}</td>
                                    <td>
                                        <c:choose>
                                            <c:when test="${usuario.ativo}">
                                                <span style="color: green;">● Ativo</span>
                                            </c:when>
                                            <c:otherwise>
                                                <span style="color: red;">● Inativo</span>
                                            </c:otherwise>
                                        </c:choose>
                                    </td>
                                </tr>
                            </c:forEach>
                        </tbody>
                    </table>

                    <p>Total de usuários: <strong>${fn:length(usuarios)}</strong></p>
                </c:when>
                <c:otherwise>
                    <p>Nenhum usuário cadastrado.</p>
                </c:otherwise>
            </c:choose>
        </div>

        <%-- Formulário com JSTL --%>
        <div class="info-box">
            <h2>📝 Adicionar Usuário</h2>
            <form action="processaUsuario.jsp" method="post">
                <table>
                    <tr>
                        <td><label for="nome">Nome:</label></td>
                        <td><input type="text" id="nome" name="nome" required></td>
                    </tr>
                    <tr>
                        <td><label for="email">Email:</label></td>
                        <td><input type="email" id="email" name="email" required></td>
                    </tr>
                    <tr>
                        <td><label for="idade">Idade:</label></td>
                        <td><input type="number" id="idade" name="idade" min="1" max="150" required></td>
                    </tr>
                    <tr>
                        <td></td>
                        <td>
                            <input type="checkbox" id="ativo" name="ativo" value="true" checked>
                            <label for="ativo">Usuário Ativo</label>
                        </td>
                    </tr>
                    <tr>
                        <td></td>
                        <td><button type="submit">Cadastrar Usuário</button></td>
                    </tr>
                </table>
            </form>
        </div>
    </div>
</body>
</html>
```

**Exemplo 14.4: Processamento de Formulários JSP**

```jsp
<%-- processaUsuario.jsp --%>
<%@ page contentType="text/html;charset=UTF-8" language="java" %>
<%@ taglib prefix="c" uri="http://java.sun.com/jsp/jstl/core" %>
<%
    // Processar os dados do formulário
    String nome = request.getParameter("nome");
    String email = request.getParameter("email");
    String idadeStr = request.getParameter("idade");
    String ativoStr = request.getParameter("ativo");

    // Validações básicas
    boolean sucesso = true;
    String mensagem = "";

    if (nome == null || nome.trim().isEmpty()) {
        sucesso = false;
        mensagem = "Nome é obrigatório";
    } else if (email == null || email.trim().isEmpty()) {
        sucesso = false;
        mensagem = "Email é obrigatório";
    } else if (idadeStr == null || idadeStr.trim().isEmpty()) {
        sucesso = false;
        mensagem = "Idade é obrigatória";
    } else {
        try {
            int idade = Integer.parseInt(idadeStr);
            boolean ativo = "true".equals(ativoStr);

            // Simular salvamento no banco de dados
            // Em uma aplicação real, isso seria feito por um DAO

            mensagem = "Usuário '" + nome + "' cadastrado com sucesso!";

        } catch (NumberFormatException e) {
            sucesso = false;
            mensagem = "Idade deve ser um número válido";
        }
    }

    // Armazenar resultado na requisição
    request.setAttribute("sucesso", sucesso);
    request.setAttribute("mensagem", mensagem);
%>

<!DOCTYPE html>
<html>
<head>
    <title>Processamento de Usuário</title>
    <style>
        body { font-family: Arial, sans-serif; margin: 40px; }
        .sucesso { background: #d4edda; color: #155724; padding: 20px; border-radius: 5px; }
        .erro { background: #f8d7da; color: #721c24; padding: 20px; border-radius: 5px; }
    </style>
</head>
<body>
    <h1>Resultado do Cadastro</h1>

    <c:choose>
        <c:when test="${sucesso}">
            <div class="sucesso">
                <h2>✅ Sucesso!</h2>
                <p>${mensagem}</p>
            </div>
        </c:when>
        <c:otherwise>
            <div class="erro">
                <h2>❌ Erro!</h2>
                <p>${mensagem}</p>
            </div>
        </c:otherwise>
    </c:choose>

    <br>
    <a href="paginaInicial.jsp">← Voltar para a página inicial</a>
</body>
</html>
```

### **14.2.4 Padrão MVC em Aplicações Web**

**Exemplo 14.5: Implementação do Padrão MVC**

```java
// Model - Classe de domínio
package com.exemplo.model;

import java.io.Serializable;
import java.time.LocalDateTime;

public class Usuario implements Serializable {
    private static final long serialVersionUID = 1L;

    private Long id;
    private String nome;
    private String email;
    private Integer idade;
    private boolean ativo;
    private LocalDateTime dataCadastro;

    // Construtores
    public Usuario() {}

    public Usuario(Long id, String nome, String email, Integer idade, boolean ativo) {
        this.id = id;
        this.nome = nome;
        this.email = email;
        this.idade = idade;
        this.ativo = ativo;
        this.dataCadastro = LocalDateTime.now();
    }

    // Getters e Setters
    public Long getId() { return id; }
    public void setId(Long id) { this.id = id; }

    public String getNome() { return nome; }
    public void setNome(String nome) { this.nome = nome; }

    public String getEmail() { return email; }
    public void setEmail(String email) { this.email = email; }

    public Integer getIdade() { return idade; }
    public void setIdade(Integer idade) { this.idade = idade; }

    public boolean isAtivo() { return ativo; }
    public void setAtivo(boolean ativo) { this.ativo = ativo; }

    public LocalDateTime getDataCadastro() { return dataCadastro; }
    public void setDataCadastro(LocalDateTime dataCadastro) { this.dataCadastro = dataCadastro; }

    @Override
    public String toString() {
        return "Usuario{id=" + id + ", nome='" + nome + "', email='" + email + "', idade=" + idade +
                ", ativo=" + ativo + ", dataCadastro=" + dataCadastro + "}";
    }
}

// Service - Lógica de negócio
package com.exemplo.service;

import com.exemplo.model.Usuario;
import java.util.*;
import java.util.concurrent.atomic.AtomicLong;

public class UsuarioService {
    private final Map<Long, Usuario> usuarios = new HashMap<>();
    private final AtomicLong contadorId = new AtomicLong(1);

    public UsuarioService() {
        // Dados iniciais para teste
        cadastrarUsuario(new Usuario(null, "João Silva", "joao.silva@email.com", 30, true));
        cadastrarUsuario(new Usuario(null, "Maria Souza", "maria.souza@email.com", 25, true));
        cadastrarUsuario(new Usuario(null, "Carlos Oliveira", "carlos.oliveira@email.com", 35, false));
    }

    public Usuario cadastrarUsuario(Usuario usuario) {
        usuario.setId(contadorId.getAndIncrement());
        usuarios.put(usuario.getId(), usuario);
        return usuario;
    }

    public List<Usuario> listarUsuarios() {
        return new ArrayList<>(usuarios.values());
    }

    public Usuario buscarPorId(Long id) {
        return usuarios.get(id);
    }

    public Usuario atualizarUsuario(Usuario usuario) {
        if (usuarios.containsKey(usuario.getId())) {
            usuarios.put(usuario.getId(), usuario);
            return usuario;
        }
        return null;
    }

    public boolean excluirUsuario(Long id) {
        return usuarios.remove(id) != null;
    }

    public List<Usuario> buscarPorNome(String nome) {
        List<Usuario> resultado = new ArrayList<>();
        for (Usuario usuario : usuarios.values()) {
            if (usuario.getNome().toLowerCase().contains(nome.toLowerCase())) {
                resultado.add(usuario);
            }
        }
        return resultado;
    }
}

// Controller - Servlet
package com.exemplo.controller;

import com.exemplo.model.Usuario;
import com.exemplo.service.UsuarioService;

import javax.servlet.*;
import javax.servlet.http.*;
import javax.servlet.annotation.*;
import java.io.IOException;
import java.util.List;

@WebServlet(name = "UsuarioController", urlPatterns = {"/usuarios"})
public class UsuarioController extends HttpServlet {

    private UsuarioService usuarioService;

    @Override
    public void init() throws ServletException {
        usuarioService = new UsuarioService();
    }

    @Override
    protected void doGet(HttpServletRequest request, HttpServletResponse response)
        throws ServletException, IOException {

        String acao = request.getParameter("acao");

        if (acao == null) {
            acao = "listar";
        }

        switch (acao) {
            case "listar":
                listarUsuarios(request, response);
                break;
            case "formCadastro":
                mostrarFormCadastro(request, response);
                break;
            case "editar":
                mostrarFormEdicao(request, response);
                break;
            case "excluir":
                excluirUsuario(request, response);
                break;
            case "buscar":
                buscarUsuarios(request, response);
                break;
            default:
                listarUsuarios(request, response);
        }
    }

    @Override
    protected void doPost(HttpServletRequest request, HttpServletResponse response)
        throws ServletException, IOException {

        String acao = request.getParameter("acao");

        if ("cadastrar".equals(acao)) {
            cadastrarUsuario(request, response);
        } else if ("atualizar".equals(acao)) {
            atualizarUsuario(request, response);
        } else {
            listarUsuarios(request, response);
        }
    }

    private void listarUsuarios(HttpServletRequest request, HttpServletResponse response)
        throws ServletException, IOException {

        List<Usuario> usuarios = usuarioService.listarUsuarios();
        request.setAttribute("usuarios", usuarios);
        request.getRequestDispatcher("/WEB-INF/views/listaUsuarios.jsp").forward(request, response);
    }

    private void mostrarFormCadastro(HttpServletRequest request, HttpServletResponse response)
        throws ServletException, IOException {

        request.getRequestDispatcher("/WEB-INF/views/formUsuario.jsp").forward(request, response);
    }

    private void mostrarFormEdicao(HttpServletRequest request, HttpServletResponse response)
        throws ServletException, IOException {

        String idStr = request.getParameter("id");
        try {
            Long id = Long.parseLong(idStr);
            Usuario usuario = usuarioService.buscarPorId(id);

            if (usuario != null) {
                request.setAttribute("usuario", usuario);
                request.getRequestDispatcher("/WEB-INF/views/formUsuario.jsp").forward(request, response);
            } else {
                request.setAttribute("erro", "Usuário não encontrado");
                listarUsuarios(request, response);
            }

        } catch (NumberFormatException e) {
            request.setAttribute("erro", "ID inválido");
            listarUsuarios(request, response);
        }
    }

    private void cadastrarUsuario(HttpServletRequest request, HttpServletResponse response)
        throws ServletException, IOException {

        try {
            String nome = request.getParameter("nome");
            String email = request.getParameter("email");
            int idade = Integer.parseInt(request.getParameter("idade"));
            boolean ativo = "on".equals(request.getParameter("ativo"));

            Usuario usuario = new Usuario();
            usuario.setNome(nome);
            usuario.setEmail(email);
            usuario.setIdade(idade);
            usuario.setAtivo(ativo);

            usuarioService.cadastrarUsuario(usuario);
            request.setAttribute("sucesso", "Usuário cadastrado com sucesso!");

        } catch (Exception e) {
            request.setAttribute("erro", "Erro ao cadastrar usuário: " + e.getMessage());
        }

        listarUsuarios(request, response);
    }

    private void atualizarUsuario(HttpServletRequest request, HttpServletResponse response)
        throws ServletException, IOException {

        try {
            Long id = Long.parseLong(request.getParameter("id"));
            String nome = request.getParameter("nome");
            String email = request.getParameter("email");
            int idade = Integer.parseInt(request.getParameter("idade"));
            boolean ativo = "on".equals(request.getParameter("ativo"));

            Usuario usuario = new Usuario();
            usuario.setId(id);
            usuario.setNome(nome);
            usuario.setEmail(email);
            usuario.setIdade(idade);
            usuario.setAtivo(ativo);

            Usuario usuarioAtualizado = usuarioService.atualizarUsuario(usuario);

            if (usuarioAtualizado != null) {
                request.setAttribute("sucesso", "Usuário atualizado com sucesso!");
            } else {
                request.setAttribute("erro", "Usuário não encontrado");
            }

        } catch (Exception e) {
            request.setAttribute("erro", "Erro ao atualizar usuário: " + e.getMessage());
        }

        listarUsuarios(request, response);
    }

    private void excluirUsuario(HttpServletRequest request, HttpServletResponse response)
        throws ServletException, IOException {

        String idStr = request.getParameter("id");
        try {
            Long id = Long.parseLong(idStr);
            boolean excluido = usuarioService.excluirUsuario(id);

            if (excluido) {
                request.setAttribute("sucesso", "Usuário excluído com sucesso!");
            } else {
                request.setAttribute("erro", "Usuário não encontrado");
            }

        } catch (NumberFormatException e) {
            request.setAttribute("erro", "ID inválido");
        }

        listarUsuarios(request, response);
    }

    private void buscarUsuarios(HttpServletRequest request, HttpServletResponse response)
        throws ServletException, IOException {

        String termo = request.getParameter("termo");
        if (termo != null && !termo.trim().isEmpty()) {
            List<Usuario> usuarios = usuarioService.buscarPorNome(termo);
            request.setAttribute("usuarios", usuarios);
            request.setAttribute("termoBusca", termo);
        } else {
            listarUsuarios(request, response);
            return;
        }

        request.getRequestDispatcher("/WEB-INF/views/listaUsuarios.jsp").forward(request, response);
    }
}
```

**Exemplo 14.6: Views JSP para o MVC**

```jsp
<%-- listaUsuarios.jsp --%>
<%@ page contentType="text/html;charset=UTF-8" language="java" %>
<%@ taglib prefix="c" uri="http://java.sun.com/jsp/jstl/core" %>
<!DOCTYPE html>
<html>
<head>
    <title>Gerenciamento de Usuários</title>
    <style>
        body { font-family: Arial, sans-serif; margin: 20px; }
        .container { max-width: 1200px; margin: 0 auto; }
        .header { background: #2c3e50; color: white; padding: 20px; border-radius: 5px; }
        .menu { margin: 20px 0; }
        .btn { background: #3498db; color: white; padding: 10px 15px; text-decoration: none; border-radius: 3px; }
        .btn-success { background: #27ae60; }
        .btn-danger { background: #e74c3c; }
        .table { width: 100%; border-collapse: collapse; margin: 20px 0; }
        .table th, .table td { border: 1px solid #ddd; padding: 12px; text-align: left; }
        .table th { background: #34495e; color: white; }
        .alert { padding: 15px; border-radius: 4px; margin: 20px 0; }
        .alert-success { background: #d4edda; color: #155724; border: 1px solid #c3e6cb; }
        .alert-danger { background: #f8d7da; color: #721c24; border: 1px solid #f5c6cb; }
        .search-form { margin: 20px 0; }
        .search-form input { padding: 8px; margin-right: 10px; }
    </style>
</head>
<body>
    <div class="container">
        <div class="header">
            <h1>👥 Gerenciamento de Usuários</h1>
            <p>Sistema de cadastro e controle de usuários</p>
        </div>

        <div class="menu">
            <a href="usuarios?acao=formCadastro" class="btn btn-success">➕ Novo Usuário</a>
            <a href="paginaInicial.jsp" class="btn">🏠 Página Inicial</a>
        </div>

        <%-- Mensagens de feedback --%>
        <c:if test="${not empty sucesso}">
            <div class="alert alert-success">
                ✅ ${sucesso}
            </div>
        </c:if>

        <c:if test="${not empty erro}">
            <div class="alert alert-danger">
                ❌ ${erro}
            </div>
        </c:if>

        <%-- Formulário de busca --%>
        <div class="search-form">
            <form action="usuarios" method="get">
                <input type="hidden" name="acao" value="buscar">
                <input type="text" name="termo" placeholder="Buscar por nome..."
                    value="${param.termo}">
                <button type="submit" class="btn">🔍 Buscar</button>
                <c:if test="${not empty termoBusca}">
                    <a href="usuarios" class="btn">🗑️ Limpar Busca</a>
                </c:if>
            </form>
        </div>

        <%-- Tabela de usuários --%>
        <c:choose>
            <c:when test="${not empty usuarios}">
                <table class="table">
                    <thead>
                        <tr>
                            <th>ID</th>
                            <th>Nome</th>
                            <th>Email</th>
                            <th>Idade</th>
                            <th>Status</th>
                            <th>Ações</th>
                        </tr>
                    </thead>
                    <tbody>
                        <c:forEach var="usuario" items="${usuarios}">
                            <tr>
                                <td>${usuario.id}</td>
                                <td>${usuario.nome}</td>
                                <td>${usuario.email}</td>
                                <td>${usuario.idade}</td>
                                <td>
                                    <c:choose>
                                        <c:when test="${usuario.ativo}">
                                            <span style="color: green; font-weight: bold;">● Ativo</span>
                                        </c:when>
                                        <c:otherwise>
                                            <span style="color: red; font-weight: bold;">● Inativo</span>
                                        </c:otherwise>
                                    </c:choose>
                                </td>
                                <td>
                                    <a href="usuarios?acao=editar&id=${usuario.id}" class="btn">✏️ Editar</a>
                                    <a href="usuarios?acao=excluir&id=${usuario.id}"
                                        class="btn btn-danger"
                                        onclick="return confirm('Tem certeza que deseja excluir este usuário?')">
                                        🗑️ Excluir
                                    </a>
                                </td>
                            </tr>
                        </c:forEach>
                    </tbody>
                </table>

                <p>Total de usuários: <strong>${fn:length(usuarios)}</strong></p>
            </c:when>
            <c:otherwise>
                <div class="alert alert-info">
                    ℹ️ Nenhum usuário encontrado.
                    <c:if test="${not empty termoBusca}">
                        Tente ajustar os termos da busca.
                    </c:if>
                </div>
            </c:otherwise>
        </c:choose>
    </div>
</body>
</html>
```

### **14.2.5 APIs REST com JAX-RS**

**Exemplo 14.7: Criando API REST**

```java
// Dependência: Jersey (implementação JAX-RS)
package com.exemplo.api;

import com.exemplo.model.Usuario;
import com.exemplo.service.UsuarioService;

import javax.ws.rs.*;
import javax.ws.rs.core.MediaType;
import javax.ws.rs.core.Response;
import java.util.List;

@Path("/api/usuarios")
@Produces(MediaType.APPLICATION_JSON)
@Consumes(MediaType.APPLICATION_JSON)
public class UsuarioResource {

    private UsuarioService usuarioService = new UsuarioService();

    @GET
    public Response listarUsuarios() {
        try {
            List<Usuario> usuarios = usuarioService.listarUsuarios();
            return Response.ok(usuarios).build();
        } catch (Exception e) {
            return Response.status(Response.Status.INTERNAL_SERVER_ERROR)
                .entity(new ErroResponse("Erro ao listar usuários: " + e.getMessage()))
                .build();
        }
    }

    @GET
    @Path("/{id}")
    public Response buscarUsuario(@PathParam("id") Long id) {
        try {
            Usuario usuario = usuarioService.buscarPorId(id);
            if (usuario != null) {
                return Response.ok(usuario).build();
            } else {
                return Response.status(Response.Status.NOT_FOUND)
                    .entity(new ErroResponse("Usuário não encontrado"))
                    .build();
            }
        } catch (Exception e) {
            return Response.status(Response.Status.INTERNAL_SERVER_ERROR)
                .entity(new ErroResponse("Erro ao buscar usuário: " + e.getMessage()))
                .build();
        }
    }

    @POST
    public Response criarUsuario(Usuario usuario) {
        try {
            if (usuario.getNome() == null || usuario.getNome().trim().isEmpty()) {
                return Response.status(Response.Status.BAD_REQUEST)
                    .entity(new ErroResponse("Nome é obrigatório"))
                    .build();
            }

            if (usuario.getEmail() == null || usuario.getEmail().trim().isEmpty()) {
                return Response.status(Response.Status.BAD_REQUEST)
                    .entity(new ErroResponse("Email é obrigatório"))
                    .build();
            }

            Usuario usuarioCriado = usuarioService.cadastrarUsuario(usuario);
            return Response.status(Response.Status.CREATED).entity(usuarioCriado).build();

        } catch (Exception e) {
            return Response.status(Response.Status.INTERNAL_SERVER_ERROR)
                .entity(new ErroResponse("Erro ao criar usuário: " + e.getMessage()))
                .build();
        }
    }

    @PUT
    @Path("/{id}")
    public Response atualizarUsuario(@PathParam("id") Long id, Usuario usuario) {
        try {
            usuario.setId(id);
            Usuario usuarioAtualizado = usuarioService.atualizarUsuario(usuario);

            if (usuarioAtualizado != null) {
                return Response.ok(usuarioAtualizado).build();
            } else {
                return Response.status(Response.Status.NOT_FOUND)
                    .entity(new ErroResponse("Usuário não encontrado"))
                    .build();
            }

        } catch (Exception e) {
            return Response.status(Response.Status.INTERNAL_SERVER_ERROR)
                .entity(new ErroResponse("Erro ao atualizar usuário: " + e.getMessage()))
                .build();
        }
    }

    @DELETE
    @Path("/{id}")
    public Response excluirUsuario(@PathParam("id") Long id) {
        try {
            boolean excluido = usuarioService.excluirUsuario(id);

            if (excluido) {
                return Response.noContent().build();
            } else {
                return Response.status(Response.Status.NOT_FOUND)
                    .entity(new ErroResponse("Usuário não encontrado"))
                    .build();
            }

        } catch (Exception e) {
            return Response.status(Response.Status.INTERNAL_SERVER_ERROR)
                .entity(new ErroResponse("Erro ao excluir usuário: " + e.getMessage()))
                .build();
        }
    }

    @GET
    @Path("/buscar")
    public Response buscarPorNome(@QueryParam("nome") String nome) {
        try {
            if (nome == null || nome.trim().isEmpty()) {
                return Response.status(Response.Status.BAD_REQUEST)
                    .entity(new ErroResponse("Parâmetro 'nome' é obrigatório"))
                    .build();
            }

            List<Usuario> usuarios = usuarioService.buscarPorNome(nome);
            return Response.ok(usuarios).build();

        } catch (Exception e) {
            return Response.status(Response.Status.INTERNAL_SERVER_ERROR)
                .entity(new ErroResponse("Erro na busca: " + e.getMessage()))
                .build();
        }
    }

    // Classe para respostas de erro padronizadas
    public static class ErroResponse {
        private String mensagem;
        private long timestamp;

        public ErroResponse(String mensagem) {
            this.mensagem = mensagem;
            this.timestamp = System.currentTimeMillis();
        }

        // Getters e Setters
        public String getMensagem() { return mensagem; }
        public void setMensagem(String mensagem) { this.mensagem = mensagem; }

        public long getTimestamp() { return timestamp; }
        public void setTimestamp(long timestamp) { this.timestamp = timestamp; }
    }
}

// Classe de configuração JAX-RS
package com.exemplo.config;

import javax.ws.rs.ApplicationPath;
import javax.ws.rs.core.Application;
import java.util.HashSet;
import java.util.Set;

@ApplicationPath("/api")
public class RestApplication extends Application {

    @Override
    public Set<Class<?>> getClasses() {
        Set<Class<?>> classes = new HashSet<>();
        classes.add(com.exemplo.api.UsuarioResource.class);
        // Adicione outros recursos REST aqui
        return classes;
    }
}
```

### **14.2.6 Segurança Web**

**Exemplo 14.8: Autenticação e Autorização**

```java
// Filtro de autenticação
package com.exemplo.security;

import javax.servlet.*;
import javax.servlet.annotation.WebFilter;
import javax.servlet.http.HttpServletRequest;
import javax.servlet.http.HttpServletResponse;
import javax.servlet.http.HttpSession;
import java.io.IOException;

@WebFilter("/*")
public class AuthenticationFilter implements Filter {

    // URLs que não requerem autenticação
    private static final String[] PUBLIC_URLS = {
        "/login", "/logout", "/public/", "/api/public/", "/css/", "/js/", "/images/"
    };

    @Override
    public void doFilter(ServletRequest request, ServletResponse response, FilterChain chain)
        throws IOException, ServletException {

        HttpServletRequest httpRequest = (HttpServletRequest) request;
        HttpServletResponse httpResponse = (HttpServletResponse) response;
        HttpSession session = httpRequest.getSession(false);

        String requestURI = httpRequest.getRequestURI();
        String contextPath = httpRequest.getContextPath();

        // Verificar se a URL é pública
        if (isPublicUrl(requestURI, contextPath)) {
            chain.doFilter(request, response);
            return;
        }

        // Verificar se o usuário está autenticado
        boolean loggedIn = session != null && session.getAttribute("usuario") != null;

        if (!loggedIn) {
            // Redirecionar para página de login
            httpResponse.sendRedirect(contextPath + "/login");
            return;
        }

        // Verificar autorização (se necessário)
        if (!hasPermission(httpRequest)) {
            httpResponse.sendError(HttpServletResponse.SC_FORBIDDEN, "Acesso negado");
            return;
        }

        chain.doFilter(request, response);
    }

    private boolean isPublicUrl(String requestURI, String contextPath) {
        String path = requestURI.substring(contextPath.length());

        for (String publicUrl : PUBLIC_URLS) {
            if (path.startsWith(publicUrl)) {
                return true;
            }
        }

        return false;
    }

    private boolean hasPermission(HttpServletRequest request) {
        // Implementar lógica de autorização baseada em roles/permissões
        // Por exemplo, verificar se o usuário tem acesso à URL específica

        HttpSession session = request.getSession(false);
        if (session != null) {
            Object usuario = session.getAttribute("usuario");
            // Verificar permissões do usuário
            return true; // Simplificado para exemplo
        }

        return false;
    }

    @Override
    public void init(FilterConfig filterConfig) throws ServletException {}

    @Override
    public void destroy() {}
}

// Servlet de login
package com.exemplo.controller;

import com.exemplo.model.Usuario;
import com.exemplo.service.UsuarioService;

import javax.servlet.*;
import javax.servlet.http.*;
import javax.servlet.annotation.*;
import java.io.IOException;

@WebServlet("/login")
public class LoginController extends HttpServlet {

    private UsuarioService usuarioService;

    @Override
    public void init() throws ServletException {
        usuarioService = new UsuarioService();
    }

    @Override
    protected void doGet(HttpServletRequest request, HttpServletResponse response)
        throws ServletException, IOException {

        // Verificar se já está logado
        HttpSession session = request.getSession(false);
        if (session != null && session.getAttribute("usuario") != null) {
            response.sendRedirect(request.getContextPath() + "/dashboard");
            return;
        }

        request.getRequestDispatcher("/WEB-INF/views/login.jsp").forward(request, response);
    }

    @Override
    protected void doPost(HttpServletRequest request, HttpServletResponse response)
        throws ServletException, IOException {

        String email = request.getParameter("email");
        String senha = request.getParameter("senha");

        // Autenticação simplificada (em produção, usar bcrypt/etc)
        boolean autenticado = autenticarUsuario(email, senha);

        if (autenticado) {
            // Criar sessão
            HttpSession session = request.getSession();
            session.setAttribute("usuario", email);
            session.setMaxInactiveInterval(30 * 60); // 30 minutos

            // Redirecionar para página inicial
            response.sendRedirect(request.getContextPath() + "/dashboard");
        } else {
            request.setAttribute("erro", "Email ou senha inválidos");
            request.getRequestDispatcher("/WEB-INF/views/login.jsp").forward(request, response);
        }
    }

    private boolean autenticarUsuario(String email, String senha) {
        // Em produção, isso seria feito com hash de senha e consulta ao banco
        return "admin@exemplo.com".equals(email) && "123456".equals(senha);
    }
}

// Servlet de logout
@WebServlet("/logout")
class LogoutController extends HttpServlet {

    @Override
    protected void doGet(HttpServletRequest request, HttpServletResponse response)
        throws ServletException, IOException {

        HttpSession session = request.getSession(false);
        if (session != null) {
            session.invalidate();
        }

        response.sendRedirect(request.getContextPath() + "/login");
    }
}
```

## **14.3 Exercícios Práticos**

**Exercício 14.1: Sistema de Blog com MVC**

```java
// Model - Post
package com.blog.model;

import java.time.LocalDateTime;
import java.util.ArrayList;
import java.util.List;

public class Post {
    private Long id;
    private String titulo;
    private String conteudo;
    private String autor;
    private LocalDateTime dataPublicacao;
    private List<String> tags;
    private boolean publicado;

    public Post() {
        this.tags = new ArrayList<>();
        this.dataPublicacao = LocalDateTime.now();
    }

    // Getters e Setters
    public Long getId() { return id; }
    public void setId(Long id) { this.id = id; }

    public String getTitulo() { return titulo; }
    public void setTitulo(String titulo) { this.titulo = titulo; }

    public String getConteudo() { return conteudo; }
    public void setConteudo(String conteudo) { this.conteudo = conteudo; }

    public String getAutor() { return autor; }
    public void setAutor(String autor) { this.autor = autor; }

    public LocalDateTime getDataPublicacao() { return dataPublicacao; }
    public void setDataPublicacao(LocalDateTime dataPublicacao) { this.dataPublicacao = dataPublicacao; }

    public List<String> getTags() { return tags; }
    public void setTags(List<String> tags) { this.tags = tags; }

    public boolean isPublicado() { return publicado; }
    public void setPublicado(boolean publicado) { this.publicado = publicado; }

    public void adicionarTag(String tag) {
        if (tag != null && !tag.trim().isEmpty()) {
            this.tags.add(tag);
        }
    }
}

// Service - PostService
package com.blog.service;

import com.blog.model.Post;
import java.util.*;
import java.util.concurrent.atomic.AtomicLong;
import java.util.stream.Collectors;

public class PostService {
    private final Map<Long, Post> posts = new HashMap<>();
    private final AtomicLong contadorId = new AtomicLong(1);

    public PostService() {
        // Posts iniciais
        Post post1 = new Post();
        post1.setId(contadorId.getAndIncrement());
        post1.setTitulo("Bem-vindo ao Blog");
        post1.setConteudo("Este é o primeiro post do nosso blog...");
        post1.setAutor("Admin");
        post1.setPublicado(true);
        post1.adicionarTag("java");
        post1.adicionarTag("blog");

        Post post2 = new Post();
        post2.setId(contadorId.getAndIncrement());
        post2.setTitulo("Introdução ao Java Web");
        post2.setConteudo("Java é uma linguagem poderosa para desenvolvimento web...");
        post2.setAutor("Admin");
        post2.setPublicado(true);
        post2.adicionarTag("java");
        post2.adicionarTag("web");
        post2.adicionarTag("servlets");

        posts.put(post1.getId(), post1);
        posts.put(post2.getId(), post2);
    }

    public Post criarPost(Post post) {
        post.setId(contadorId.getAndIncrement());
        posts.put(post.getId(), post);
        return post;
    }

    public List<Post> listarPosts() {
        return new ArrayList<>(posts.values());
    }

    public List<Post> listarPostsPublicados() {
        return posts.values().stream()
            .filter(Post::isPublicado)
            .sorted((p1, p2) -> p2.getDataPublicacao().compareTo(p1.getDataPublicacao()))
            .collect(Collectors.toList());
    }

    public Post buscarPorId(Long id) {
        return posts.get(id);
    }

    public Post atualizarPost(Post post) {
        if (posts.containsKey(post.getId())) {
            posts.put(post.getId(), post);
            return post;
        }
        return null;
    }

    public boolean excluirPost(Long id) {
        return posts.remove(id) != null;
    }

    public List<Post> buscarPorTag(String tag) {
        return posts.values().stream()
            .filter(p -> p.isPublicado() && p.getTags().contains(tag.toLowerCase()))
            .collect(Collectors.toList());
    }

    public List<Post> buscarPorAutor(String autor) {
        return posts.values().stream()
            .filter(p -> p.isPublicado() && p.getAutor().equalsIgnoreCase(autor))
            .collect(Collectors.toList());
    }
}

// Controller - PostController
package com.blog.controller;

import com.blog.model.Post;
import com.blog.service.PostService;

import javax.servlet.*;
import javax.servlet.http.*;
import javax.servlet.annotation.*;
import java.io.IOException;
import java.util.Arrays;
import java.util.List;

@WebServlet(name = "PostController", urlPatterns = {"/posts", "/blog"})
public class PostController extends HttpServlet {

    private PostService postService;

    @Override
    public void init() throws ServletException {
        postService = new PostService();
    }

    @Override
    protected void doGet(HttpServletRequest request, HttpServletResponse response)
        throws ServletException, IOException {

        String acao = request.getParameter("acao");
        String path = request.getServletPath();

        if ("/blog".equals(path)) {
            // Site público
            if (acao == null) acao = "listarPublicos";
        }

        if (acao == null) {
            acao = "listar";
        }

        switch (acao) {
            case "listar":
                listarPosts(request, response);
                break;
            case "listarPublicos":
                listarPostsPublicos(request, response);
                break;
            case "visualizar":
                visualizarPost(request, response);
                break;
            case "formCadastro":
                mostrarFormCadastro(request, response);
                break;
            case "editar":
                mostrarFormEdicao(request, response);
                break;
            case "buscar":
                buscarPosts(request, response);
                break;
            default:
                listarPostsPublicos(request, response);
        }
    }

    @Override
    protected void doPost(HttpServletRequest request, HttpServletResponse response)
        throws ServletException, IOException {

        String acao = request.getParameter("acao");

        if ("cadastrar".equals(acao)) {
            cadastrarPost(request, response);
        } else if ("atualizar".equals(acao)) {
            atualizarPost(request, response);
        } else {
            listarPosts(request, response);
        }
    }

    private void listarPosts(HttpServletRequest request, HttpServletResponse response)
        throws ServletException, IOException {

        List<Post> posts = postService.listarPosts();
        request.setAttribute("posts", posts);
        request.getRequestDispatcher("/WEB-INF/views/admin/listaPosts.jsp").forward(request, response);
    }

    private void listarPostsPublicos(HttpServletRequest request, HttpServletResponse response)
        throws ServletException, IOException {

        List<Post> posts = postService.listarPostsPublicados();
        request.setAttribute("posts", posts);
        request.getRequestDispatcher("/WEB-INF/views/blog/listaPostsPublicos.jsp").forward(request, response);
    }

    private void visualizarPost(HttpServletRequest request, HttpServletResponse response)
        throws ServletException, IOException {

        String idStr = request.getParameter("id");
        try {
            Long id = Long.parseLong(idStr);
            Post post = postService.buscarPorId(id);

            if (post != null && post.isPublicado()) {
                request.setAttribute("post", post);
                request.getRequestDispatcher("/WEB-INF/views/blog/detalhePost.jsp").forward(request, response);
            } else {
                request.setAttribute("erro", "Post não encontrado ou não publicado");
                listarPostsPublicos(request, response);
            }

        } catch (NumberFormatException e) {
            request.setAttribute("erro", "ID inválido");
            listarPostsPublicos(request, response);
        }
    }

    private void mostrarFormCadastro(HttpServletRequest request, HttpServletResponse response)
        throws ServletException, IOException {

        request.getRequestDispatcher("/WEB-INF/views/admin/formPost.jsp").forward(request, response);
    }

    private void mostrarFormEdicao(HttpServletRequest request, HttpServletResponse response)
        throws ServletException, IOException {

        String idStr = request.getParameter("id");
        try {
            Long id = Long.parseLong(idStr);
            Post post = postService.buscarPorId(id);

            if (post != null) {
                request.setAttribute("post", post);
                request.getRequestDispatcher("/WEB-INF/views/admin/formPost.jsp").forward(request, response);
            } else {
                request.setAttribute("erro", "Post não encontrado");
                listarPosts(request, response);
            }

        } catch (NumberFormatException e) {
            request.setAttribute("erro", "ID inválido");
            listarPosts(request, response);
        }
    }

    private void cadastrarPost(HttpServletRequest request, HttpServletResponse response)
        throws ServletException, IOException {

        try {
            String titulo = request.getParameter("titulo");
            String conteudo = request.getParameter("conteudo");
            String autor = request.getParameter("autor");
            String tags = request.getParameter("tags");
            boolean publicado = "on".equals(request.getParameter("publicado"));

            Post post = new Post();
            post.setTitulo(titulo);
            post.setConteudo(conteudo);
            post.setAutor(autor);
            post.setPublicado(publicado);

            // Processar tags
            if (tags != null && !tags.trim().isEmpty()) {
                String[] tagsArray = tags.split(",");
                for (String tag : tagsArray) {
                    post.adicionarTag(tag.trim().toLowerCase());
                }
            }

            postService.criarPost(post);
            request.setAttribute("sucesso", "Post cadastrado com sucesso!");

        } catch (Exception e) {
            request.setAttribute("erro", "Erro ao cadastrar post: " + e.getMessage());
        }

        listarPosts(request, response);
    }

    private void atualizarPost(HttpServletRequest request, HttpServletResponse response)
        throws ServletException, IOException {

        try {
            Long id = Long.parseLong(request.getParameter("id"));
            String titulo = request.getParameter("titulo");
            String conteudo = request.getParameter("conteudo");
            String autor = request.getParameter("autor");
            String tags = request.getParameter("tags");
            boolean publicado = "on".equals(request.getParameter("publicado"));

            Post post = new Post();
            post.setId(id);
            post.setTitulo(titulo);
            post.setConteudo(conteudo);
            post.setAutor(autor);
            post.setPublicado(publicado);

            // Processar tags
            if (tags != null && !tags.trim().isEmpty()) {
                String[] tagsArray = tags.split(",");
                for (String tag : tagsArray) {
                    post.adicionarTag(tag.trim().toLowerCase());
                }
            }

            Post postAtualizado = postService.atualizarPost(post);

            if (postAtualizado != null) {
                request.setAttribute("sucesso", "Post atualizado com sucesso!");
            } else {
                request.setAttribute("erro", "Post não encontrado");
            }

        } catch (Exception e) {
            request.setAttribute("erro", "Erro ao atualizar post: " + e.getMessage());
        }

        listarPosts(request, response);
    }

    private void buscarPosts(HttpServletRequest request, HttpServletResponse response)
        throws ServletException, IOException {

        String tipo = request.getParameter("tipo");
        String termo = request.getParameter("termo");

        List<Post> resultados;

        if ("tag".equals(tipo) && termo != null && !termo.trim().isEmpty()) {
            resultados = postService.buscarPorTag(termo);
            request.setAttribute("tipoBusca", "tag");
            request.setAttribute("termoBusca", termo);
        } else if ("autor".equals(tipo) && termo != null && !termo.trim().isEmpty()) {
            resultados = postService.buscarPorAutor(termo);
            request.setAttribute("tipoBusca", "autor");
            request.setAttribute("termoBusca", termo);
        } else {
            resultados = postService.listarPostsPublicados();
        }

        request.setAttribute("posts", resultados);
        request.getRequestDispatcher("/WEB-INF/views/blog/listaPostsPublicos.jsp").forward(request, response);
    }
}
```

## **14.4 Resumo do Módulo**

### **Pontos Principais:**

- **Servlets**: Componentes Java para processar requisições HTTP no servidor
- **JSP**: Tecnologia para criar páginas web dinâmicas com Java
- **MVC**: Padrão arquitetural para separar concerns (Model-View-Controller)
- **JAX-RS**: Especificação para criar APIs RESTful em Java
- **Segurança**: Autenticação, autorização e proteção contra vulnerabilidades web
- **Sessões**: Mecanismo para manter estado entre requisições HTTP

### **Dicas para Desenvolvimento Web:**

- Use o padrão MVC para organizar sua aplicação
- Prefira JSTL e Expression Language sobre scriptlets em JSP
- Implemente tratamento de erros adequado
- Use prepared statements para prevenir SQL injection
- Valide dados tanto no cliente quanto no servidor
- Implemente mecanismos de segurança (autenticação, CSRF protection)

**Próximo Módulo: Tópicos Avançados e Preparação para a Certificação**

Preparado para revisar os tópicos mais avançados e se preparar para a prova de certificação Java SE 17 Developer?

---

# **Módulo 15: Tópicos Avançados e Preparação para a Certificação**

## **15.1 Objetivos do Módulo**

- Revisar tópicos avançados da linguagem Java
- Dominar conceitos complexos para a certificação
- Praticar com questões no estilo da prova
- Desenvolver estratégias para a realização do exame
- Consolidar todo o conhecimento necessário

## **15.2 Conteúdo Programático**

### **15.2.1 Tópicos Avançados de Java**

**Exemplo 15.1: Métodos Default e Privados em Interfaces**

```java
import java.util.*;
import java.util.function.*;

public class InterfacesAvancadas {

    // Interface com métodos default, private e estáticos
    interface ProcessadorTexto {
        // Método abstrato tradicional
        String processar(String texto);

        // Método default (Java 8+)
        default String processarMaiusculo(String texto) {
            validarTexto(texto);
            return processar(texto).toUpperCase();
        }

        default String processarMinusculo(String texto) {
            validarTexto(texto);
            return processar(texto).toLowerCase();
        }

        // Método privado (Java 9+) - reutilização interna
        private void validarTexto(String texto) {
            if (texto == null || texto.trim().isEmpty()) {
                throw new IllegalArgumentException("Texto não pode ser nulo ou vazio");
            }
        }

        // Método estático em interface
        static ProcessadorTexto criarProcessadorSimples() {
            return texto -> texto.replace(" ", "-");
        }

        static ProcessadorTexto criarProcessadorReverso() {
            return texto -> new StringBuilder(texto).reverse().toString();
        }
    }

    // Implementação da interface
    static class ProcessadorCustomizado implements ProcessadorTexto {
        @Override
        public String processar(String texto) {
            return ">>> " + texto.trim() + " <<<";
        }

        // Pode sobrescrever métodos default se necessário
        @Override
        public String processarMaiusculo(String texto) {
            return "UPPER: " + processar(texto).toUpperCase();
        }
    }

    // Herança múltipla de interfaces
    interface Validavel {
        default void validar() {
            System.out.println("Validação básica");
        }
    }

    interface Logavel {
        default void log(String mensagem) {
            System.out.println("LOG: " + mensagem);
        }

        // Conflito de métodos default
        default void processar() {
            System.out.println("Processamento genérico");
        }
    }

    static class ServicoCompleto implements Validavel, Logavel {
        // Deve resolver o conflito de métodos default
        @Override
        public void processar() {
            Validavel.super.processar(); // Chamada explícita
            Logavel.super.processar(); // Chamada explícita
            System.out.println("Processamento customizado");
        }
    }

    public static void main(String[] args) {
        System.out.println("=== INTERFACES AVANÇADAS ===");

        // Usando método estático da interface
        ProcessadorTexto simples = ProcessadorTexto.criarProcessadorSimples();
        ProcessadorTexto reverso = ProcessadorTexto.criarProcessadorReverso();

        System.out.println("Simples: " + simples.processar("Hello World"));
        System.out.println("Reverso: " + reverso.processar("Java"));
        System.out.println("Maiúsculo: " + simples.processarMaiusculo("teste"));

        // Processador customizado
        ProcessadorTexto custom = new ProcessadorCustomizado();
        System.out.println("Custom: " + custom.processar(" texto com espaços "));
        System.out.println("Custom Upper: " + custom.processarMaiusculo("teste"));

        // Herança múltipla
        ServicoCompleto servico = new ServicoCompleto();
        servico.validar();
        servico.log("Mensagem de teste");
        servico.processar();
    }
}

// Interfaces funcionais complexas
class InterfacesFuncionaisAvancadas {

    public static void main(String[] args) {
        System.out.println("\n=== INTERFACES FUNCIONAIS AVANÇADADAS ===");

        // Function composition
        Function<String, Integer> paraInteiro = Integer::parseInt;
        Function<Integer, String> paraString = Object::toString;
        Function<String, String> composicao = paraInteiro.andThen(paraString);

        System.out.println("Composição: " + composicao.apply("123"));

        // Predicate composition
        Predicate<String> naoVazio = s -> s != null && !s.isEmpty();
        Predicate<String> longo = s -> s.length() > 5;
        Predicate<String> valido = naoVazio.and(longo);

        System.out.println("Valido 'teste': " + valido.test("teste"));
        System.out.println("Valido 'teste longo': " + valido.test("teste longo"));

        // Supplier com lazy evaluation
        Supplier<Double> numeroAleatorio = () -> {
            double numero = Math.random();
            System.out.println("Gerando número: " + numero);
            return numero;
        };

        System.out.println("Supplier lazy:");
        System.out.println("Número 1: " + numeroAleatorio.get());
        System.out.println("Número 2: " + numeroAleatorio.get());

        // Consumer chain
        Consumer<String> imprimir = System.out::println;
        Consumer<String> upperCase = s -> System.out.println(s.toUpperCase());
        Consumer<String> ambos = imprimir.andThen(upperCase);

        ambos.accept("java certification");
    }
}
```

### **15.2.2 Generics Avançados**

**Exemplo 15.2: Generics Complexos e Type Erasure**

```java
import java.util.*;
import java.lang.reflect.*;

public class GenericsAvancados {

    // Classe genérica com múltiplos tipos e restrições
    static class ParOrdenado<K extends Comparable<K> & Serializable,
                            V extends Cloneable> {
        private final K chave;
        private V valor;

        public ParOrdenado(K chave, V valor) {
            this.chave = chave;
            this.valor = valor;
        }

        public K getChave() { return chave; }
        public V getValor() { return valor; }
        public void setValor(V valor) { this.valor = valor; }

        // Método genérico em classe genérica
        public <T> T processarChave(Function<K, T> funcao) {
            return funcao.apply(chave);
        }

        // Wildcard com upper bound em método
        public void processarLista(List<? extends V> lista) {
            for (V elemento : lista) {
                System.out.println("Processando: " + elemento);
            }
        }

        // Wildcard com lower bound
        public void adicionarALista(List<? super V> lista) {
            lista.add(valor);
        }
    }

    // Herança com generics
    static class ParNumerico<N extends Number> extends ParOrdenado<String, N> {
        public ParNumerico(String chave, N valor) {
            super(chave, valor);
        }

        public double getValorDouble() {
            return getValor().doubleValue();
        }
    }

    // Generic array creation (cuidado!)
    @SuppressWarnings("unchecked")
    static class Colecao<T> {
        private T[] elementos;
        private int tamanho;

        public Colecao(Class<T> tipo, int capacidade) {
            // Maneira correta de criar array genérico
            this.elementos = (T[]) Array.newInstance(tipo, capacidade);
            this.tamanho = 0;
        }

        public void adicionar(T elemento) {
            if (tamanho < elementos.length) {
                elementos[tamanho++] = elemento;
            }
        }

        public T[] getElementos() {
            return Arrays.copyOf(elementos, tamanho);
        }
    }

    // Demonstração de type erasure
    public static void demonstrarTypeErasure() {
        System.out.println("=== TYPE ERASURE ===");

        List<String> listaStrings = new ArrayList<>();
        List<Integer> listaInteiros = new ArrayList<>();

        // Type erasure - em runtime ambos são List<Object>
        System.out.println("Tipo listaStrings: " + listaStrings.getClass());
        System.out.println("Tipo listaInteiros: " + listaInteiros.getClass());
        System.out.println("Mesmo tipo? " +
                (listaStrings.getClass() == listaInteiros.getClass()));

        // Reflexão e generics
        try {
            Method metodo = Colecao.class.getMethod("adicionar", Object.class);
            Type[] tiposParametros = metodo.getGenericParameterTypes();
            System.out.println("Tipo parâmetro: " + tiposParametros[0]);
        } catch (Exception e) {
            e.printStackTrace();
        }
    }

    // Bridge methods
    interface Comparavel<T> {
        int comparar(T outro);
    }

    static class StringComparavel implements Comparavel<String> {
        @Override
        public int comparar(String outro) {
            return this.toString().compareTo(outro);
        }

        // O compilador cria um método bridge:
        // public int comparar(Object outro) {
        //     return comparar((String) outro);
        // }
    }

    // Generic method com wildcard complexo
    public static <T> void copiarLista(List<? extends T> fonte,
                                      List<? super T> destino) {
        for (T elemento : fonte) {
            destino.add(elemento);
        }
    }

    // Intersection types com generics
    public static <T extends Comparable<T> & Serializable> T max(T a, T b) {
        return a.compareTo(b) >= 0 ? a : b;
    }

    public static void main(String[] args) {
        System.out.println("=== GENERICS AVANÇADOS ===");

        // Par ordenado complexo
        ParOrdenado<String, ArrayList<String>> par =
            new ParOrdenado<>("config", new ArrayList<>());

        par.getValor().add("item1");
        par.getValor().add("item2");

        // Processamento com função
        Integer tamanho = par.processarChave(String::length);
        System.out.println("Tamanho da chave: " + tamanho);

        // Par numérico
        ParNumerico<Integer> parNum = new ParNumerico<>("idade", 25);
        System.out.println("Valor como double: " + parNum.getValorDouble());

        // Coleção com array genérico
        Colecao<String> colecao = new Colecao<>(String.class, 10);
        colecao.adicionar("A");
        colecao.adicionar("B");
        System.out.println("Array: " + Arrays.toString(colecao.getElementos()));

        demonstrarTypeErasure();

        // Cópia com wildcards
        List<Integer> fonte = Arrays.asList(1, 2, 3);
        List<Number> destino = new ArrayList<>();
        copiarLista(fonte, destino);
        System.out.println("Lista copiada: " + destino);
    }
}
```

### **15.2.3 Concorrência Avançada**

**Exemplo 15.3: Padrões Avançados de Concorrência**

```java
import java.util.concurrent.*;
import java.util.concurrent.atomic.*;
import java.util.concurrent.locks.*;
import java.util.*;

public class ConcorrenciaAvancada {

    // Atomic classes para operações atômicas
    static class ContadorAtomico {
        private final AtomicLong contador = new AtomicLong(0);
        private final AtomicReference<String> ultimoValor =
            new AtomicReference<>("Nenhum");
        private final AtomicIntegerArray arrayAtomico =
            new AtomicIntegerArray(10);

        public void incrementar() {
            long novoValor = contador.incrementAndGet();
            ultimoValor.set("Incrementado para: " + novoValor);

            // Atualizar array atômico
            int index = (int) (novoValor % arrayAtomico.length());
            arrayAtomico.getAndIncrement(index);
        }

        public long getContador() {
            return contador.get();
        }

        public boolean compararESet(long esperado, long novo) {
            return contador.compareAndSet(esperado, novo);
        }

        public void imprimirEstado() {
            System.out.println("Contador: " + contador.get());
            System.out.println("Último valor: " + ultimoValor.get());
            System.out.println("Array: " + arrayAtomico);
        }
    }

    // Lock-free algorithm com CAS (Compare-And-Swap)
    static class PilhaLockFree<T> {
        private static class Node<T> {
            final T valor;
            volatile Node<T> proximo;

            Node(T valor) {
                this.valor = valor;
            }
        }

        private final AtomicReference<Node<T>> topo =
            new AtomicReference<>();

        public void push(T valor) {
            Node<T> novoNo = new Node<>(valor);
            Node<T> topoAtual;
            do {
                topoAtual = topo.get();
                novoNo.proximo = topoAtual;
            } while (!topo.compareAndSet(topoAtual, novoNo));
        }

        public T pop() {
            Node<T> topoAtual;
            Node<T> novoTopo;
            do {
                topoAtual = topo.get();
                if (topoAtual == null) {
                    return null;
                }
                novoTopo = topoAtual.proximo;
            } while (!topo.compareAndSet(topoAtual, novoTopo));

            return topoAtual.valor;
        }

        public boolean isEmpty() {
            return topo.get() == null;
        }
    }

    // StampedLock para leituras otimistas
    static class DadosCompartilhados {
        private final StampedLock lock = new StampedLock();
        private String dados;
        private int versao;

        public void atualizar(String novosDados) {
            long stamp = lock.writeLock();
            try {
                dados = novosDados;
                versao++;
                System.out.println("Dados atualizados para: " + novosDados);
            } finally {
                lock.unlockWrite(stamp);
            }
        }

        public String ler() {
            long stamp = lock.readLock();
            try {
                return dados + " (v" + versao + ")";
            } finally {
                lock.unlockRead(stamp);
            }
        }

        public String lerOtimista() {
            long stamp = lock.tryOptimisticRead();
            String dadosAtuais = dados;
            int versaoAtual = versao;

            if (!lock.validate(stamp)) {
                // Leitura otimista falhou, usar leitura bloqueante
                stamp = lock.readLock();
                try {
                    dadosAtuais = dados;
                    versaoAtual = versao;
                } finally {
                    lock.unlockRead(stamp);
                }
            }

            return dadosAtuais + " (v" + versaoAtual + ") [otimista]";
        }
    }

    // CompletableFuture avançado
    static class ProcessamentoAssincrono {

        public CompletableFuture<String> processarEmParalelo(String entrada) {
            return CompletableFuture.supplyAsync(() -> {
                System.out.println("Processamento 1 iniciado...");
                try { Thread.sleep(1000); } catch (InterruptedException e) {}
                return entrada.toUpperCase();
            })
            .thenApplyAsync(resultado -> {
                System.out.println("Processamento 2 iniciado...");
                try { Thread.sleep(500); } catch (InterruptedException e) {}
                return resultado + " - PROCESSADO";
            })
            .thenComposeAsync(resultado -> {
                System.out.println("Processamento 3 iniciado...");
                return CompletableFuture.supplyAsync(() ->
                    resultado.replace(" ", "_"));
            })
            .exceptionally(erro -> {
                System.err.println("Erro no processamento: " + erro.getMessage());
                return "VALOR_PADRAO";
            });
        }

        public CompletableFuture<Void> processarMultiplasTarefas() {
            List<CompletableFuture<String>> futures = Arrays.asList(
                CompletableFuture.supplyAsync(() -> "Tarefa A"),
                CompletableFuture.supplyAsync(() -> "Tarefa B"),
                CompletableFuture.supplyAsync(() -> "Tarefa C")
            );

            return CompletableFuture.allOf(futures.toArray(new CompletableFuture[0]))
                .thenRun(() -> {
                    System.out.println("Todas as tarefas completadas");
                    futures.forEach(future -> {
                        try {
                            System.out.println("Resultado: " + future.get());
                        } catch (Exception e) {
                            e.printStackTrace();
                        }
                    });
                });
        }
    }

    // ExecutorService customizado com ThreadFactory
    static class ExecutorPersonalizado {
        private final ExecutorService executor;
        private final AtomicInteger contadorThreads;

        public ExecutorPersonalizado() {
            this.contadorThreads = new AtomicInteger(1);
            this.executor = Executors.newFixedThreadPool(3, runnable -> {
                Thread thread = new Thread(runnable);
                thread.setName("Worker-" + contadorThreads.getAndIncrement());
                thread.setDaemon(true);
                thread.setUncaughtExceptionHandler((t, e) -> {
                    System.err.println("Erro não tratado na thread " + t.getName() + ": " + e.getMessage());
                });
                return thread;
            });
        }

        public <T> CompletableFuture<T> executar(Callable<T> tarefa) {
            return CompletableFuture.supplyAsync(() -> {
                try {
                    return tarefa.call();
                } catch (Exception e) {
                    throw new RuntimeException(e);
                }
            }, executor);
        }

        public void shutdown() {
            executor.shutdown();
            try {
                if (!executor.awaitTermination(5, TimeUnit.SECONDS)) {
                    executor.shutdownNow();
                }
            } catch (InterruptedException e) {
                executor.shutdownNow();
                Thread.currentThread().interrupt();
            }
        }
    }

    public static void main(String[] args) throws Exception {
        System.out.println("=== CONCORRÊNCIA AVANÇADA ===");

        // Contador atômico
        ContadorAtomico contador = new ContadorAtomico();
        ExecutorService executor = Executors.newFixedThreadPool(5);

        for (int i = 0; i < 10; i++) {
            executor.execute(contador::incrementar);
        }

        executor.shutdown();
        executor.awaitTermination(1, TimeUnit.SECONDS);
        contador.imprimirEstado();

        // Pilha lock-free
        PilhaLockFree<String> pilha = new PilhaLockFree<>();
        pilha.push("A");
        pilha.push("B");
        pilha.push("C");
        System.out.println("Pop: " + pilha.pop());
        System.out.println("Pop: " + pilha.pop());

        // StampedLock
        DadosCompartilhados dados = new DadosCompartilhados();
        dados.atualizar("Valor Inicial");

        ExecutorService leitores = Executors.newFixedThreadPool(3);
        for (int i = 0; i < 5; i++) {
            leitores.execute(() -> {
                System.out.println("Leitura: " + dados.lerOtimista());
            });
        }
        leitores.shutdown();

        // CompletableFuture avançado
        ProcessamentoAssincrono processador = new ProcessamentoAssincrono();
        CompletableFuture<String> future = processador.processarEmParalelo("hello world");
        future.thenAccept(resultado ->
            System.out.println("Resultado final: " + resultado));

        processador.processarMultiplasTarefas().get();

        // Executor personalizado
        ExecutorPersonalizado personalizado = new ExecutorPersonalizado();
        personalizado.executar(() -> "Tarefa personalizada")
            .thenAccept(System.out::println);

        personalizado.shutdown();

        Thread.sleep(2000); // Aguardar processamento assíncrono
    }
}
```

### **15.2.4 Performance e Otimização**

**Exemplo 15.4: Técnicas de Otimização em Java**

```java
import java.util.*;
import java.lang.management.*;
import java.nio.charset.StandardCharsets;

public class PerformanceOtimizacao {

    // Gerenciamento de memória e GC
    static class GerenciamentoMemoria {
        public static void monitorarMemoria() {
            MemoryMXBean memoryBean = ManagementFactory.getMemoryMXBean();
            MemoryUsage heapUsage = memoryBean.getHeapMemoryUsage();
            MemoryUsage nonHeapUsage = memoryBean.getNonHeapMemoryUsage();

            System.out.println("=== MONITORAMENTO DE MEMÓRIA ===");
            System.out.printf("Heap: %d / %d MB (usado/max)%n",
                heapUsage.getUsed() / 1024 / 1024,
                heapUsage.getMax() / 1024 / 1024);
            System.out.printf("Non-Heap: %d / %d MB (usado/max)%n",
                nonHeapUsage.getUsed() / 1024 / 1024,
                nonHeapUsage.getMax() / 1024 / 1024);

            // Sugerir GC (apenas sugestão!)
            System.gc();
        }

        public static void demonstrarStringVsBuilder() {
            int iteracoes = 10000;

            // String concatenation (ineficiente)
            long inicio = System.currentTimeMillis();
            String resultado = "";
            for (int i = 0; i < iteracoes; i++) {
                resultado += i; // Cria novo objeto a cada iteração
            }
            long fim = System.currentTimeMillis();
            System.out.printf("String concatenation: %d ms%n", fim - inicio);

            // StringBuilder (eficiente)
            inicio = System.currentTimeMillis();
            StringBuilder sb = new StringBuilder();
            for (int i = 0; i < iteracoes; i++) {
                sb.append(i);
            }
            resultado = sb.toString();
            fim = System.currentTimeMillis();
            System.out.printf("StringBuilder: %d ms%n", fim - inicio);
        }
    }

    // Cache de objetos para reduzir alocação
    static class ObjectPool<T> {
        private final Queue<T> pool;
        private final Supplier<T> creator;
        private final Consumer<T> resetter;

        public ObjectPool(int tamanho, Supplier<T> creator, Consumer<T> resetter) {
            this.pool = new LinkedList<>();
            this.creator = creator;
            this.resetter = resetter;

            for (int i = 0; i < tamanho; i++) {
                pool.offer(creator.get());
            }
        }

        public T borrow() {
            T obj = pool.poll();
            if (obj == null) {
                obj = creator.get();
            }
            return obj;
        }

        public void returnObject(T obj) {
            resetter.accept(obj);
            pool.offer(obj);
        }
    }

    // Byte operations para performance
    static class ProcessamentoBytes {
        public static int calcularChecksum(byte[] dados) {
            int checksum = 0;
            for (byte b : dados) {
                checksum ^= b & 0xFF; // Evitar extensão de sinal
            }
            return checksum;
        }

        public static byte[] compactarDados(String texto) {
            // Simulação de compactação
            return texto.getBytes(StandardCharsets.UTF_8);
        }

        public static String descompactarDados(byte[] dados) {
            return new String(dados, StandardCharsets.UTF_8);
        }
    }

    // Otimização de loops
    static class OtimizacaoLoops {
        public static int somaArrayIneficiente(int[] array) {
            int soma = 0;
            for (int i = 0; i < array.length; i++) {
                soma += array[i]; // Acesso por índice
            }
            return soma;
        }

        public static int somaArrayEficiente(int[] array) {
            int soma = 0;
            for (int valor : array) {
                soma += valor; // Acesso direto
            }
            return soma;
        }

        public static void loopUnrolling(int[] array) {
            // Desenrolar loop para reduzir overhead
            int i = 0;
            int soma = 0;
            for (; i <= array.length - 4; i += 4) {
                soma += array[i];
                soma += array[i + 1];
                soma += array[i + 2];
                soma += array[i + 3];
            }

            // Processar elementos restantes
            for (; i < array.length; i++) {
                soma += array[i];
            }
        }
    }

    // Enum com métodos específicos para performance
    enum TipoOperacao {
        SOMA {
            @Override
            public int aplicar(int a, int b) {
                return a + b;
            }
        },
        SUBTRACAO {
            @Override
            public int aplicar(int a, int b) {
                return a - b;
            }
        },
        MULTIPLICACAO {
            @Override
            public int aplicar(int a, int b) {
                return a * b;
            }
        };

        public abstract int aplicar(int a, int b);
    }

    // JIT Compiler optimizations
    static class JitOptimizations {
        // Método que pode ser inline pelo JIT
        public static final int calcular(int x, int y) {
            return x * y + x - y;
        }

        // Constant folding
        public static final int CONSTANTE = 42 * 100; // Calculado em compile-time

        // Dead code elimination
        public static void metodoComDeadCode() {
            if (false) { // Eliminado pelo compilador
                System.out.println("Este código nunca será executado");
            }
        }

        // Loop hoisting
        public static int somaComLoopHoisting(int[] array, int constante) {
            int soma = 0;
            for (int valor : array) {
                soma += valor * constante; // constante é "hoisted" para fora do loop
            }
            return soma;
        }
    }

    // Memory-mapped files para I/O de alta performance
    static class HighPerformanceIO {
        // Em produção, usar java.nio.channels.FileChannel com map()
        public static void demonstrarEficiencia() {
            List<String> lines = Arrays.asList("linha1", "linha2", "linha3");

            // Approach tradicional
            long start = System.nanoTime();
            try {
                // Código de escrita de arquivo...
            } catch (Exception e) {
                e.printStackTrace();
            }
            long end = System.nanoTime();
            System.out.printf("I/O tradicional: %d ns%n", end - start);

            // Approach com buffer
            start = System.nanoTime();
            StringBuilder buffer = new StringBuilder();
            for (String line : lines) {
                buffer.append(line).append("\n");
            }
            // Escrever buffer de uma vez
            end = System.nanoTime();
            System.out.printf("I/O com buffer: %d ns%n", end - start);
        }
    }

    public static void main(String[] args) {
        System.out.println("=== PERFORMANCE E OTIMIZAÇÃO ===");

        GerenciamentoMemoria.monitorarMemoria();
        GerenciamentoMemoria.demonstrarStringVsBuilder();

        // Object pool
        ObjectPool<StringBuilder> pool = new ObjectPool<>(
            5,
            StringBuilder::new,
            sb -> sb.setLength(0)
        );

        StringBuilder sb1 = pool.borrow();
        sb1.append("Hello");
        System.out.println("StringBuilder do pool: " + sb1.toString());
        pool.returnObject(sb1);

        // Processamento de bytes
        byte[] dados = ProcessamentoBytes.compactarDados("Teste de performance");
        int checksum = ProcessamentoBytes.calcularChecksum(dados);
        System.out.println("Checksum: " + checksum);

        // Otimização de loops
        int[] array = new int[1000];
        Arrays.fill(array, 1);

        long start = System.nanoTime();
        OtimizacaoLoops.somaArrayIneficiente(array);
        long end = System.nanoTime();
        System.out.printf("Loop ineficiente: %d ns%n", end - start);

        start = System.nanoTime();
        OtimizacaoLoops.somaArrayEficiente(array);
        end = System.nanoTime();
        System.out.printf("Loop eficiente: %d ns%n", end - start);

        // Enum performance
        int resultado = TipoOperacao.SOMA.aplicar(10, 5);
        System.out.println("Resultado operação: " + resultado);

        // JIT optimizations
        int calc = JitOptimizations.calcular(10, 20);
        System.out.println("Cálculo JIT: " + calc);

        HighPerformanceIO.demonstrarEficiencia();
    }
}
```

### **15.2.5 Questões de Certificação - Estilo Prova**

**Exemplo 15.5: Questões no Estilo da Prova**

```java
import java.util.*;
import java.util.function.*;
import java.util.stream.*;

public class QuestoesCertificacao {

    // Questão 1: Streams e Lambdas
    public static void questaoStreams() {
        System.out.println("=== QUESTÃO 1: STREAMS ===");

        List<String> palavras = Arrays.asList("java", "certification", "exam", "preparation");

        // Qual é o resultado?
        String resultado = palavras.stream()
            .filter(s -> s.length() > 4)
            .map(String::toUpperCase)
            .sorted()
            .collect(Collectors.joining(", "));

        System.out.println("Resultado: " + resultado);
        // a) JAVA, CERTIFICATION, PREPARATION
        // b) CERTIFICATION, PREPARATION
        // c) CERTIFICATION, EXAM, PREPARATION
        // d) exam, java, preparation
    }

    // Questão 2: Concorrência
    public static void questaoConcorrencia() {
        System.out.println("\n=== QUESTÃO 2: CONCORRÊNCIA ===");

        AtomicInteger contador = new AtomicInteger(0);
        ExecutorService executor = Executors.newFixedThreadPool(2);

        Runnable tarefa = () -> {
            for (int i = 0; i < 1000; i++) {
                contador.incrementAndGet();
            }
        };

        executor.execute(tarefa);
        executor.execute(tarefa);
        executor.shutdown();

        try {
            executor.awaitTermination(1, TimeUnit.SECONDS);
        } catch (InterruptedException e) {
            Thread.currentThread().interrupt();
        }

        System.out.println("Contador: " + contador.get());
        // a) Sempre 2000
        // b) Entre 1000 e 2000
        // c) Sempre 1000
        // d) Pode ser qualquer valor
    }

    // Questão 3: Collections e Generics
    public static void questaoCollections() {
        System.out.println("\n=== QUESTÃO 3: COLLECTIONS ===");

        List<Integer> numeros = new ArrayList<>();
        numeros.add(1);
        numeros.add(2);
        numeros.add(3);

        // O que acontece?
        for (Integer numero : numeros) {
            if (numero == 2) {
                numeros.remove(numero); // ConcurrentModificationException?
            }
        }

        System.out.println("Lista: " + numeros);
        // a) [1, 3]
        // b) [1, 2, 3]
        // c) ConcurrentModificationException
        // d) NullPointerException
    }

    // Questão 4: Interfaces Funcionais
    public static void questaoInterfacesFuncionais() {
        System.out.println("\n=== QUESTÃO 4: INTERFACES FUNCIONAIS ===");

        Function<String, Integer> func1 = Integer::parseInt;
        Function<Integer, String> func2 = Object::toString;

        // Qual é o resultado?
        Function<String, String> composicao = func1.andThen(func2);
        String resultado = composicao.apply("123");

        System.out.println("Resultado: " + resultado);
        // a) 123
        // b) "123"
        // c) ClassCastException
        // d) NumberFormatException
    }

    // Questão 5: Exceções
    public static void questaoExcecoes() {
        System.out.println("\n=== QUESTÃO 5: EXCEÇÕES ===");

        try {
            System.out.println("Início try");
            if (true) throw new RuntimeException("Erro 1");
            System.out.println("Fim try"); // Nunca executado
        } catch (RuntimeException e) {
            System.out.println("Catch: " + e.getMessage());
            throw new RuntimeException("Erro 2");
        } finally {
            System.out.println("Finally executado");
        }

        // Qual a saída?
        // a) Início try, Catch: Erro 1, Finally executado, RuntimeException: Erro 2
        // b) Início try, Catch: Erro 1, Finally executado
        // c) Início try, Finally executado, RuntimeException: Erro 1
        // d) Início try, Catch: Erro 1, RuntimeException: Erro 2
    }

    // Questão 6: Modularidade (Java 9+)
    public static void questaoModularidade() {
        System.out.println("\n=== QUESTÃO 6: MODULARIDADE ===");

        // Qual afirmação sobre module-info.java é CORRETA?
        System.out.println("Opções:");
        System.out.println("a) Um módulo deve exportar todos os seus pacotes");
        System.out.println("b) 'requires transitive' torna a dependência visível para usuários do módulo");
        System.out.println("c) 'exports to' restringe as exportações para módulos específicos");
        System.out.println("d) Todas as anteriores");

        // Resposta: b e c são corretas
    }

    // Questão 7: Pattern Matching (Java 17)
    public static void questaoPatternMatching() {
        System.out.println("\n=== QUESTÃO 7: PATTERN MATCHING ===");

        Object obj = "Java 17";

        // Pattern matching com instanceof
        if (obj instanceof String s && s.length() > 5) {
            System.out.println("String longa: " + s.toUpperCase());
        } else {
            System.out.println("Não é string longa");
        }

        // Qual é a saída?
        // a) String longa: JAVA 17
        // b) Não é string longa
        // c) Compilation error
        // d) Runtime exception
    }

    // Questão 8: Records (Java 16+)
    public static void questaoRecords() {
        System.out.println("\n=== QUESTÃO 8: RECORDS ===");

        record Pessoa(String nome, int idade) {
            public Pessoa {
                if (idade < 0) throw new IllegalArgumentException("Idade inválida");
            }

            public String nomeMaiusculo() {
                return nome.toUpperCase();
            }
        }

        Pessoa p = new Pessoa("João", 25);
        System.out.println("Nome: " + p.nomeMaiusculo());
        System.out.println("Idade: " + p.idade());
        System.out.println("ToString: " + p.toString());

        // Quais afirmações são verdadeiras sobre records?
        // a) São imutáveis
        // b) Geram automaticamente equals(), hashCode(), toString()
        // c) Podem ter métodos adicionais
        // d) Todas as anteriores
    }

    // Questão 9: Optional Avançado
    public static void questaoOptional() {
        System.out.println("\n=== QUESTÃO 9: OPTIONAL ===");

        Optional<String> opt = Optional.of("valor");

        // Qual é o resultado?
        String resultado = opt
            .filter(s -> s.length() > 10)
            .or(() -> Optional.of("padrão"))
            .map(String::toUpperCase)
            .get();

        System.out.println("Resultado: " + resultado);
        // a) "VALOR"
        // b) "PADRÃO"
        // c) NoSuchElementException
        // d) Optional["PADRÃO"]
    }

    // Questão 10: DateTime API
    public static void questaoDateTime() {
        System.out.println("\n=== QUESTÃO 10: DATE/TIME API ===");

        var data = java.time.LocalDate.of(2024, 1, 15);
        var novaData = data.plusMonths(2).minusDays(10);

        System.out.println("Nova data: " + novaData);
        // a) 2024-03-05
        // b) 2024-03-15
        // c) 2024-02-05
        // d) 2024-02-15
    }

    public static void main(String[] args) {
        questaoStreams();
        questaoConcorrencia();
        questaoCollections();
        questaoInterfacesFuncionais();
        questaoExcecoes();
        questaoModularidade();
        questaoPatternMatching();
        questaoRecords();
        questaoOptional();
        questaoDateTime();

        System.out.println("\n=== RESPOSTAS ===");
        System.out.println("1: b) CERTIFICATION, PREPARATION");
        System.out.println("2: a) Sempre 2000 (AtomicInteger é thread-safe)");
        System.out.println("3: c) ConcurrentModificationException");
        System.out.println("4: b) \"123\"");
        System.out.println("5: a) Início try, Catch: Erro 1, Finally executado, RuntimeException: Erro 2");
        System.out.println("6: b e c são corretas");
        System.out.println("7: a) String longa: JAVA 17");
        System.out.println("8: d) Todas as anteriores");
        System.out.println("9: b) \"PADRÃO\"");
        System.out.println("10: a) 2024-03-05");
    }
}
```

### **15.2.6 Estratégias para a Prova**

**Exemplo 15.6: Preparação Final e Dicas**

```java
import java.util.*;

public class EstrategiasProva {

    // Checklist de tópicos para revisar
    public static class ChecklistCertificacao {
        private final Map<String, Boolean> topicos = new LinkedHashMap<>();

        public ChecklistCertificacao() {
            // Tópicos essenciais da certificação Java SE 17
            topicos.put("Java Basics and Data Types", false);
            topicos.put("Control Flow Statements", false);
            topicos.put("Object-Oriented Programming", false);
            topicos.put("Exceptions and Assertions", false);
            topicos.put("Arrays and Collections", false);
            topicos.put("Streams and Lambda Expressions", false);
            topicos.put("Java Platform Module System", false);
            topicos.put("Concurrency", false);
            topicos.put("I/O and NIO.2", false);
            topicos.put("JDBC and Database", false);
            topicos.put("Localization", false);
            topicos.put("Annotations", false);
            topicos.put("Generics and Collections", false);
            topicos.put("Functional Programming", false);
            topicos.put("Sealed Classes and Records", false);
            topicos.put("Pattern Matching", false);
        }

        public void marcarComoRevisado(String topico) {
            if (topicos.containsKey(topico)) {
                topicos.put(topico, true);
            }
        }

        public void imprimirProgresso() {
            System.out.println("=== CHECKLIST DE REVISÃO ===");
            long revisados = topicos.values().stream().filter(b -> b).count();
            double percentual = (double) revisados / topicos.size() * 100;

            System.out.printf("Progresso: %.1f%% (%d/%d)%n",
                percentual, revisados, topicos.size());

            topicos.forEach((topico, revisado) -> {
                String status = revisado ? "✓" : "✗";
                System.out.printf("%s %s%n", status, topico);
            });
        }
    }

    // Simulador de ambiente de prova
    public static class SimuladorProva {
        private static final int TEMPO_TOTAL = 180; // 3 horas em minutos
        private static final int TOTAL_QUESTOES = 80;

        public void simularProva() {
            System.out.println("\n=== SIMULAÇÃO DE PROVA ===");
            System.out.println("Tempo total: " + TEMPO_TOTAL + " minutos");
            System.out.println("Total de questões: " + TOTAL_QUESTOES);
            System.out.println("Tempo médio por questão: " +
                (TEMPO_TOTAL * 60 / TOTAL_QUESTOES) + " segundos");

            System.out.println("\nEstratégias recomendadas:");
            System.out.println("1. Comece pelas questões mais fáceis");
            System.out.println("2. Marque as difíceis para revisar depois");
            System.out.println("3. Controle o tempo - não fique travado em uma questão");
            System.out.println("4. Revise as marcadas nos últimos 30 minutos");
            System.out.println("5. Cuidado com questões 'truque'");
        }

        public void dicasEspecificas() {
            System.out.println("\n=== DICAS ESPECÍFICAS ===");

            List<String> dicas = Arrays.asList(
                "✅ Preste atenção em modificadores de acesso (public, private, protected)",
                "✅ Entenda bem polymorphism e overriding vs overloading",
                "✅ Conheça todas as exceções unchecked e checked",
                "✅ Domine a ordem de inicialização de classes e instâncias",
                "✅ Pratique questões com generics e wildcards",
                "✅ Entenda bem lambda expressions e method references",
                "✅ Conheça as operações intermediárias e terminais de Streams",
                "✅ Estude o comportamento de Collections (List, Set, Map)",
                "✅ Entenda thread safety e problemas de concorrência",
                "✅ Conheça as novas features do Java 17 (records, sealed classes, etc)",
                "✅ Pratique reading comprehension - muitas questões são longas",
                "✅ Cuidado com null pointer exceptions em cadeias de métodos",
                "✅ Entenda bem try-with-resources e ordem de fechamento",
                "✅ Conheça a diferença entre == e equals()",
                "✅ Domine o uso de Optional e seus métodos"
            );

            dicas.forEach(System.out::println);
        }
    }

    // Gerenciador de estudos
    public static class GerenciadorEstudos {
        private final Map<String, Integer> tempoPorTopico = new HashMap<>();
        private int tempoTotalEstudado = 0;

        public void registrarEstudo(String topico, int minutos) {
            tempoPorTopico.merge(topico, minutos, Integer::sum);
            tempoTotalEstudado += minutos;
        }

        public void gerarRelatorio() {
            System.out.println("\n=== RELATÓRIO DE ESTUDOS ===");
            System.out.println("Tempo total estudado: " + tempoTotalEstudado + " minutos");

            System.out.println("\nTempo por tópico:");
            tempoPorTopico.entrySet().stream()
                .sorted(Map.Entry.<String, Integer>comparingByValue().reversed())
                .forEach(entry ->
                    System.out.printf("- %s: %d minutos%n", entry.getKey(), entry.getValue()));

            // Sugerir tópicos para revisar
            System.out.println("\nTópicos sugeridos para revisão:");
            tempoPorTopico.entrySet().stream()
                .sorted(Map.Entry.comparingByValue())
                .limit(3)
                .forEach(entry ->
                    System.out.printf("- %s (apenas %d minutos)%n",
                        entry.getKey(), entry.getValue()));
        }
    }

    // Questões mais frequentes na prova
    public static class TopicosMaisTestados {
        public static List<String> getTopicosFrequentes() {
            return Arrays.asList(
                "Lambda Expressions and Functional Interfaces",
                "Stream API Operations",
                "Collections Framework (List, Set, Map)",
                "Exception Handling",
                "Concurrency (Threads, Executors)",
                "Java I/O and NIO.2",
                "JDBC and Database Connectivity",
                "Generics and Type Erasure",
                "Object-Oriented Principles",
                "Java Module System"
            );
        }

        public static void imprimirTopicosFrequentes() {
            System.out.println("\n=== TÓPICOS MAIS FREQUENTES NA PROVA ===");
            List<String> topicos = getTopicosFrequentes();
            for (int i = 0; i < topicos.size(); i++) {
                System.out.printf("%d. %s%n", i + 1, topicos.get(i));
            }
        }
    }

    public static void main(String[] args) {
        System.out.println("=== ESTRATÉGIAS PARA A PROVA DE CERTIFICAÇÃO ===");

        // Checklist
        ChecklistCertificacao checklist = new ChecklistCertificacao();
        checklist.marcarComoRevisado("Java Basics and Data Types");
        checklist.marcarComoRevisado("Control Flow Statements");
        checklist.marcarComoRevisado("Object-Oriented Programming");
        checklist.imprimirProgresso();

        // Simulador de prova
        SimuladorProva simulador = new SimuladorProva();
        simulador.simularProva();
        simulador.dicasEspecificas();

        // Gerenciador de estudos
        GerenciadorEstudos gerenciador = new GerenciadorEstudos();
        gerenciador.registrarEstudo("Streams", 120);
        gerenciador.registrarEstudo("Concurrency", 90);
        gerenciador.registrarEstudo("Collections", 60);
        gerenciador.gerarRelatorio();

        // Tópicos frequentes
        TopicosMaisTestados.imprimirTopicosFrequentes();

        // Mensagem final
        System.out.println("\n=== MENSAGEM FINAL ===");
        System.out.println("🎯 Você está bem preparado!");
        System.out.println("📚 Continue praticando com questões similares à prova");
        System.out.println("⏰ Descanse bem antes da prova");
        System.out.println("🍀 Boa sorte na sua certificação Java SE 17!");
    }
}
```

## **15.3 Resumo do Curso Completo**

### **O que Cobrimos:**

1. **Fundamentos Java**: Sintaxe, tipos de dados, operadores
2. **Controle de Fluxo**: Estruturas de decisão e repetição
3. **OOP**: Classes, objetos, herança, polimorfismo
4. **Tratamento de Exceções**: Try-catch, custom exceptions
5. **Collections**: List, Set, Map, Queue
6. **Generics**: Type safety, wildcards
7. **Functional Programming**: Lambdas, Streams
8. **Concorrência**: Threads, Executors, Synchronization
9. **I/O e NIO.2**: File operations, streams
10. **JDBC**: Database connectivity, transactions
11. **Desenvolvimento Web**: Servlets, JSP, MVC
12. **Tópicos Avançados**: Performance, patterns, best practices

### **Próximos Passos Recomendados:**

1. **Pratique com simulados oficiais**
2. **Revise os tópicos onde tem mais dificuldade**
3. **Crie projetos práticos para consolidar o conhecimento**
4. **Participe de fóruns e comunidades Java**
5. **Considere outras certificações (Spring, Cloud, etc.)**

## **Parabéns por completar o curso!** 🎉

Você agora tem uma base sólida em Java SE 17 e está bem preparado para a certificação. Continue praticando e aprofundando seus conhecimentos.
