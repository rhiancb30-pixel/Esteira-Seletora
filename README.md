# Esteira Seletora Linear

## 📌 Descrição do Projeto

Este repositório apresenta o desenvolvimento de uma **Esteira Seletora Linear**, criada como projeto didático para o Curso de Engenharia Mecatrônica do **Instituto Federal de Santa Catarina (IFSC)**, no contexto da disciplina **Projeto Integrador Eletromecânico**.

O objetivo principal do projeto é proporcionar aos alunos uma experiência prática próxima à realidade industrial, integrando conceitos de **mecânica, eletrônica e programação**, por meio de um sistema automatizado, modular e de baixo custo.

A esteira é capaz de **transportar, identificar, contar e separar peças metálicas e não metálicas**, exibindo informações de funcionamento em uma interface homem-máquina (IHM) com display LCD.

---

## 🎯 Objetivos

* Desenvolver um equipamento didático inspirado em sistemas industriais reais;
* Aplicar conhecimentos multidisciplinares (mecânica, eletrônica e programação);
* Criar uma solução **modular**, **expansível** e **replicável**;
* Disponibilizar **documentação aberta** para uso e aprimoramento por outros estudantes.

---

## ⚙️ Funcionalidades Principais

* Transporte contínuo de peças por esteira;
* Contagem total de peças;
* Identificação de peças metálicas;
* Separação automática das peças por meio de servo motor;
* Exibição de dados no display LCD (quantidade de peças, estado do motor);
* Arquitetura modular, permitindo a adição de novos sensores e atuadores.

---

## 🧩 Arquitetura do Sistema

O sistema é dividido em dois módulos principais:

### 🔹 Caixa Elétrica

* Arduino Mega (controlador principal);
* Display LCD 16x2 com interface I2C;
* Botões de controle;
* Placa de circuito impresso (PCB);
* Fonte de alimentação 12 V;

### 🔹 Esteira Seletora

* Estrutura em acrílico e perfis de alumínio;
* Motor de passo com driver TB6600;
* Servo motor SG90 para separação;
* Sensor capacitivo (contagem);
* Sensor indutivo (detecção de metal);
* Lona em PVC e roletes impressos em 3D.

---

## 🛠️ Tecnologias Utilizadas

### Hardware

* Arduino Mega
* Motor de passo + Driver TB6600
* Servo motor SG90
* Sensor capacitivo
* Sensor indutivo
* Display LCD 16x2 (I2C)

### Software

* Linguagem **C++** (Arduino)
* Bibliotecas:

  * `AccelStepper`
  * `Servo`
  * `LiquidCrystal_I2C`

### Ferramentas

* SolidWorks (modelagem mecânica)
* Proteus (esquemático e PCB)
* Impressão 3D (peças estruturais)
* Corte a laser (acrílico)

---

## 📂 Estrutura do Repositório (sugerida)

```
Esteira-Seletora-Linear/
│
├── Documentação/
│   └── Projeto_Integrador.pdf        # Relatório final do projeto (ou versão em .docx)
│
├── Imagens do Projeto/
│   ├── prototipo_montado.jpg
│   ├── caixa_eletrica.jpg
│   ├── esteira_montada.jpg
│   └── esquematico_geral.png
│
├── Desenho técnico/
│   ├── Caixa/
│   │   ├── tampa_caixa.pdf
│   │   ├── lateral_caixa.pdf
│   │   └── base_caixa.pdf
│   │
│   └── Esteira/
│       ├── lateral_esteira.pdf
│       ├── eixo_motor.pdf
│       ├── eixo_movido.pdf
│       └── seletor_servo.pdf
│
├── dxf/
│   ├── caixa/
│   │   └── *.dxf                     # Arquivos DXF para corte a laser
│   └── esteira/
│       └── *.dxf
│
├── stl/
│   ├── cantoneiras/
│   │   └── *.stl                     # Peças impressas em 3D
│   ├── roletes/
│   │   └── *.stl
│   └── suportes/
│       └── *.stl
│
├── Eletronica PI/
│   ├── pcb/
│   │   └── layout_pcb.pdf
│   └── componentes/
│       └── lista_componentes.xlsx
│
├── Proteus/
│   ├── Esquematico1/
│   │   └── *.pdsprj                  # Versões iniciais / testes
│   │
│   └── EsquematicoPI/
│       └── *.pdsprj                  # Esquemático final do projeto
│
├── firmware/
│   └── esteira_seletora.ino           # Código Arduino
│
├── README.md
└── LICENSE

```

---

## 🚀 Como Utilizar

1. Monte a estrutura mecânica conforme os desenhos técnicos;
2. Realize a montagem elétrica com base no esquemático;
3. Carregue o código no Arduino Mega;
4. Ajuste sensores e atuadores conforme a aplicação;
5. Utilize o sistema em atividades didáticas ou como base para novos projetos.

---

## 🔧 Possíveis Melhorias Futuras

* Adição de sensor de cor RGB;
* Implementação de sistema de visão computacional;
* Classificação por múltiplos critérios (material + cor);
* Modularização da eletrônica em placas dedicadas;
* Integração com CLP para uso em aulas avançadas.

---

## 👨‍💻 Autores

* Alex Gabriel Claure Escobar
* Elisa Klosinski dos Santos
* Helio Henrique Hinckel Filho
* Rhian Eric Cabral Branco

---

## 🏫 Instituição

**Instituto Federal de Santa Catarina (IFSC)**
Curso Técnico Integrado ao Ensino Médio em Mecatrônica
Projeto Integrador Eletromecânico – 2025

---

## 📜 Licença

Este projeto é disponibilizado para fins **educacionais e acadêmicos**. Sinta-se à vontade para estudar, adaptar e evoluir a solução, citando os autores e a instituição quando aplicável.
