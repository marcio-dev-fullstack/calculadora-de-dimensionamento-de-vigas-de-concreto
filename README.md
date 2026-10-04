<div align="center">

# 🎓 Gerador e Validador de Quiz Educacional (DIP-EDU-01)

[![Java](https://img.shields.io/badge/Java-17%2B-orange?style=for-the-badge&logo=openjdk&logoColor=white)](https://www.oracle.com/java/)
[![Spring Boot](https://img.shields.io/badge/Spring_Boot-3.x-green?style=for-the-badge&logo=spring&logoColor=white)](https://spring.io/projects/spring-boot)
[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg?style=for-the-badge)](https://opensource.org/licenses/MIT)
[![Status](https://img.shields.io/badge/Status-Em_Desenvolvimento-yellow?style=for-the-badge)]()

*Sistema centralizado para gestão, aplicação e correção automatizada de avaliações educacionais.*

**Gerente e Desenvolvedor Responsável:** Márcio Rodrigues de Oliveira

</div>

---

## 📌 Visão Geral do Projeto

O **Gerador e Validador de Quiz Educacional** é uma solução robusta projetada para modernizar o processo avaliativo em instituições de ensino e centros de treinamento técnico. O sistema elimina a correção manual e a tabulação demorada em planilhas, oferecendo um fluxo automatizado de ponta a ponta: desde o cadastro de itens em banco de dados até a exportação de relatórios analíticos de desempenho.

---

## 🚀 Funcionalidades Principais

* **🗂️ Banco de Questões:** Cadastro flexível de perguntas de múltipla escolha com suporte a níveis de dificuldade, pesos, tags e alternativas customizáveis.
* **⏱️ Aplicação Cronometrada:** Interface de teste intuitiva para o aluno com temporizador regressivo e salvamento de estado atômico.
* **⚡ Correção Instantânea:** Motor lógico que compara as respostas submetidas com o gabarito oficial em milissegundos.
* **📊 Relatórios e Métricas:** Painel de aproveitamento para docentes com exportação de resultados em formatos padronizados (`PDF` e `CSV`).

---

## 🛠️ Stack Tecnológica

O projeto foi arquitetado utilizando padrões modernos de desenvolvimento de software:

* **Linguagem:** Java (JDK 17+)
* **Framework:** Spring Boot / Spring MVC / Thymeleaf (ou JavaFX para versão desktop nativa)
* **Persistência de Dados:** H2 Database (Modo Embarcado) / SQLite
* **Geração de Documentos:** Apache PDFBox (para relatórios em PDF)
* **Arquitetura:** Padrão em Camadas (Controller / Service / Repository) alinhado aos princípios SOLID.

---

## 🏗️ Arquitetura e Estrutura de Camadas

```text
src/main/java/com/marcioliveira/quiz
│
├── controller/     # Controladores de rotas e requisições HTTP / GUI
├── service/        # Regras de negócio (Correção, Embaralhamento, Validação)
├── repository/     # Camada de persistência e acesso a dados (JPA / JDBC)
├── model/          # Entidades de Domínio (Quiz, Questao, Aluno, Submissao)
└── dto/            # Objetos de Transferência de Dados
```

---

## 📋 Requisitos do Sistema

### Requisitos Funcionais
* **RF01:** Cadastro de questões vinculadas a disciplinas e categorias por usuários com perfil docente.
* **RF02:** Criação de provas personalizadas com limite de tempo e pontuação total ajustável.
* **RF03:** Exibição controlada de questões com cronômetro ativo para o discente.
* **RF04:** Cálculo e persistência automática da nota final imediatamente após a submissão.

### Requisitos Não Funcionais
* **RNF01:** Tempo de resposta para correção e submissão inferior a 1 segundo.
* **RNF02:** Persistência atômica de dados para evitar perda de avaliações em caso de falhas abruptas.

---

## ⚙️ Como Executar o Projeto

1. **Pré-requisitos:**
   * Ter o **Java JDK 17+** instalado em sua máquina.
   * Ter o **Maven** configurado no PATH.

2. **Clonar o Repositório:**
   ```bash
   git clone https://github.com/seu-usuario/quiz-educacional-java.git
   cd quiz-educacional-java
   ```

3. **Compilar e Executar:**
   ```bash
   mvn clean spring-boot:run
   ```

4. **Acessar a Aplicação:**
   Abra o navegador e acesse: `http://localhost:8080`

---

## 📄 Licença

Este projeto é distribuído sob a licença MIT. Veja o arquivo `LICENSE` para mais detalhes.

---
<div align="center">
Desenvolvido com dedicação por <strong>Márcio Rodrigues de Oliveira</strong>.
</div>
