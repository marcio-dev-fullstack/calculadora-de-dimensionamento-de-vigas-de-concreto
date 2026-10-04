<div align="center">

# 🏗️ Calculadora de Dimensionamento de Vigas de Concreto (DIP-ENG-02)

[![C#](https://img.shields.io/badge/C%23-.NET_8-purple?style=for-the-badge&logo=csharp&logoColor=white)](https://dotnet.microsoft.com/)
[![WPF](https://img.shields.io/badge/WPF-Windows_Presentation_Foundation-blue?style=for-the-badge&logo=windows&logoColor=white)](https://docs.microsoft.com/en-us/dotnet/desktop/wpf/)
[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg?style=for-the-badge)](https://opensource.org/licenses/MIT)
[![Status](https://img.shields.io/badge/Status-Em_Desenvolvimento-yellow?style=for-the-badge)]()

*Ferramenta computacional de alta performance para cálculo estrutural e dimensionamento de armaduras em vigas de concreto armado.*

**Gerente e Desenvolvedor Responsável:** Márcio Rodrigues de Oliveira

</div>

---

## 📌 Visão Geral do Projeto

O **DIP-ENG-02** é uma solução desktop moderna e intuitiva projetada para auxiliar engenheiros civis, calculistas e estudantes de engenharia na fase de projeto estrutural. O aplicativo automatiza o dimensionamento de armaduras longitudinais e transversais em vigas submetidas à flexão simples e esforço cortante, garantindo conformidade com as normas técnicas vigentes (como a ABNT NBR 6118) e eliminando erros manuais de cálculo e consulta tabular.

---

## 🚀 Funcionalidades Principais

* **📐 Entrada Paramétrica Completa:** Configuração ágil de dados geométricos ($b$, $h$, cobrimento) e mecânicos ($f_{ck}$ do concreto, $f_{yk}$ do aço).
* **⚡ Motor de Cálculo Iterativo:** Determinação automatizada da linha neutra ($x$), verificação de domínios de deformação (Domínios 2, 3 e 4) e cálculo exato da área de aço necessária ($As$).
* **🔗 Dimensionamento de Estribos:** Cálculo da armadura transversal para combate ao esforço cortante ($V_{sd}$).
* **📊 Relatório Técnico Integrado:** Emissão de sumários descritivos e memoriais de cálculo prontos para conferência e cópia.

---

## 🛠️ Stack Tecnológica

O projeto foi construído utilizando o ecossistema moderno da Microsoft:

* **Linguagem:** C# (.NET 8)
* **Interface Gráfica (GUI):** WPF (Windows Presentation Foundation) com arquitetura reativa baseada em padrões MVVM.
* **Persistência de Dados (Opcional):** SQLite embarcado para histórico local de projetos estruturais.
* **Arquitetura:** Padrão limpo desacoplando a lógica de negócio estrutural da interface de usuário.

---

## 🏗️ Estrutura da Arquitetura

```text
src/
├── Core/               # Modelos matemáticos e regras normativas de cálculo
├── ViewModels/         # Lógica de apresentação e comandos MVVM
├── Views/              # Interfaces gráficas em XAML (WPF)
└── Services/           # Serviços de exportação de relatórios e persistência local
```

---

## 📋 Critérios Técnicos e Normativos

O motor de cálculo segue rigorosamente os princípios fundamentais do projeto de estruturas de concreto:
* **Flexão Simples:** Verificação dos limites de escoamento do aço e deformação máxima do concreto (ruptura frágil x dúctil).
* **Domínios de Deformação:** Classificação estrutural de acordo com a NBR 6118.
* **Taxas de Armadura:** Alertas automáticos para valores inferiores ao mínimo exigido por norma ou superiores ao limite máximo de esmagamento das bielas comprimidas.

---

## ⚙️ Como Executar o Projeto

1. **Pré-requisitos:**
   * Ter o [.NET 8 SDK](https://dotnet.microsoft.com/download/dotnet/8.0) instalado.
   * Sistema Operacional Windows (recomendado para execução nativa WPF).

2. **Clonar o Repositório:**
   ```bash
   git clone https://github.com/seu-usuario/calculadora-vigas-concreto.git
   cd calculadora-vigas-concreto
   ```

3. **Compilar e Executar:**
   ```bash
   dotnet build
   dotnet run --project src/Views/ConcreteBeamCalculator.csproj
   ```

---

## 📄 Licença

Este projeto é distribuído sob a licença MIT. Consulte o arquivo `LICENSE` para mais detalhes.

---
<div align="center">
Desenvolvido com rigor técnico por <strong>Márcio Rodrigues de Oliveira</strong>.
</div>
