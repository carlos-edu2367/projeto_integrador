Projeto Calculadora Java com Testes JUnit 5 e Controle de Versão com Git/GitHub
1. Introdução
Este projeto Java simula o desenvolvimento de um módulo de software simples: uma calculadora. O foco principal está na aplicação de boas práticas de testes automatizados com JUnit 5 e no gerenciamento de código utilizando controle de versão com Git e GitHub. O objetivo é demonstrar a implementação de testes unitários e funcionais, bem como a configuração e gerenciamento de um repositório Git, incluindo práticas de branching e merge para simular um fluxo de trabalho de desenvolvimento colaborativo.

Este repositório pode ser acessado em: https://github.com/carlos-edu2367/projeto_integrador

2. Funcionalidades da Calculadora
A classe Calculadora implementa as quatro operações aritméticas básicas:

somar(double a, double b): Realiza a adição de dois números.

subtrair(double a, double b): Realiza a subtração de dois números.

multiplicar(double a, double b): Realiza a multiplicação de dois números.

dividir(double a, double b): Realiza a divisão de dois números. Lança uma ArithmeticException caso o divisor seja zero, garantindo a robustez da aplicação.

3. Testes Automatizados com JUnit 5
Para garantir a qualidade e a corretude das funcionalidades da calculadora, foram implementados testes unitários e funcionais utilizando o framework JUnit 5. A classe CalculadoraTest cobre diferentes cenários de uso para cada operação, incluindo:

testSoma(): Verifica a soma de números positivos, negativos e zero.

testSubtracao(): Verifica a subtração de números positivos, negativos e zero.

testMultiplicacao(): Verifica a multiplicação de números positivos, negativos e zero.

testDivisao(): Verifica a divisão de números positivos e negativos.

testDivisaoPorZero(): Testa o cenário crucial de divisão por zero, garantindo que a ArithmeticException esperada seja corretamente lançada.

4. Estrutura do Projeto
A estrutura de diretórios do projeto é organizada da seguinte forma:

.
├── src/main/java/
│   └── Calculadora.java  # Contém a lógica da calculadora
├── src/test/java/
│   └── CalculadoraTest.java # Contém todos os testes unitários para a calculadora
├── pom.xml               # Arquivo de configuração Maven para gerenciar dependências e build
└── README.md             # Este arquivo, que documenta o projeto

5. Como Executar os Testes
Para compilar e executar os testes automatizados deste projeto, siga os passos abaixo. Este projeto utiliza Maven para gerenciamento de dependências.

Clone o repositório:
Abra seu terminal ou prompt de comando e clone o projeto para sua máquina local usando o comando:

git clone https://github.com/carlos-edu2367/projeto_integrador

Navegue até o diretório do projeto:

cd projeto_integrador

Execute os testes:
Utilize o Maven para compilar o projeto e rodar todos os testes definidos na classe CalculadoraTest:

mvn clean test

Alternativamente, se estiver utilizando uma IDE (como IntelliJ IDEA, Eclipse ou VS Code com extensões Java), você pode executar os testes diretamente da IDE, clicando com o botão direito na classe CalculadoraTest e selecionando a opção para rodar os testes JUnit.

6. Controle de Versão com Git e GitHub
Este projeto adere às boas práticas de controle de versão, utilizando Git para o gerenciamento detalhado do histórico de código e o GitHub como plataforma de repositório remoto.

6.1. Ramificação (Branching)
O desenvolvimento de novas funcionalidades, como a própria calculadora, foi realizado em branches dedicadas (por exemplo, feature/calculadora). Essa abordagem isola as mudanças, permitindo um desenvolvimento seguro e sem interferências na branch principal (main) até que a funcionalidade esteja completamente desenvolvida, testada e pronta para integração.

6.2. Commits
Commits são realizados de forma regular e incremental, com mensagens claras e descritivas. Cada commit representa uma unidade lógica de trabalho, facilitando o rastreamento de alterações, a revisão de código e a compreensão do histórico de desenvolvimento do projeto.

6.3. Fusão (Merge)
Após a conclusão e validação da funcionalidade em sua branch de desenvolvimento, as alterações são integradas à branch main através de um processo de merge. Este processo garante que o código final, revisado e testado, seja incorporado à linha principal do projeto.

7. Pré-requisitos
Para trabalhar com este projeto, você precisará ter instalado em sua máquina:

Java Development Kit (JDK): Versão 11 ou superior.

Apache Maven: Para gerenciamento de dependências e construção do projeto.

Git: Para controle de versão.

Conta no GitHub: Para acessar e gerenciar o repositório remoto.

8. Contribuição (Fluxo de Trabalho Colaborativo)
Embora este seja um projeto individual, ele foi desenvolvido seguindo um fluxo de trabalho que simula um ambiente colaborativo. Para futuras extensões ou colaborações, o processo recomendado seria:

Fork do Repositório: Se você for um colaborador externo, crie um fork deste repositório para sua conta do GitHub.

Clone o Fork: Clone seu fork para sua máquina local.

Crie uma Nova Branch: Para cada nova funcionalidade ou correção, crie uma branch específica: git checkout -b feature/sua-nova-funcionalidade ou git checkout -b bugfix/correcao-do-bug.

Desenvolva e Teste: Implemente suas alterações, sempre adicionando ou atualizando os testes JUnit conforme necessário.

Comite Suas Alterações: Faça commits com mensagens claras e concisas.

Envie para o GitHub: Envie sua branch para o seu repositório remoto: git push origin feature/sua-nova-funcionalidade.

Abra um Pull Request: No GitHub, abra um Pull Request (PR) da sua branch para a branch main do repositório original, descrevendo suas mudanças e os testes realizados.