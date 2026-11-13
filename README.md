# PSE-em-Acao
AEP 2 semestre.
## Sistema de Planejamento e Acompanhamento de Ações de Saúde na Escola

Projeto desenvolvido como parte da Atividade de Estudo Programada (AEP) do curso de Análise e Desenvolvimento de Sistemas da Universidade Cesumar – UNICESUMAR.

## Objetivo

Desenvolver uma aplicação em linguagem C para auxiliar no planejamento,
registro e acompanhamento de ações coletivas do Programa Saúde na Escola (PSE).

## Integrantes

- Nome do integrante 1: Murilo Alexandre de Assis/RA:26010057-2
- Nome do integrante 2: Arthur Mingroni Pacheco/RA:26006047-2
- Nome do integrante 3: Joelson Batista dos Santos/RA:26012817-2

## Sobre o projeto

O sistema terá como objetivo organizar informações relacionadas às ações
coletivas do PSE, permitindo cadastrar, listar, pesquisar e atualizar ações,
além de gerar um resumo geral das atividades.

## Funcionalidades planejadas

1. Cadastro de ações;
2. Listagem das ações cadastradas;
3. Pesquisa por código, escola ou tema;
4. Atualização da situação da ação;
5. Registro da quantidade efetiva de participantes;
6. Geração de resumo geral;
7. Validação das entradas.

## Tecnologias

- Linguagem C
- GitHub
- Fluxogramas
- Pseudocódigo

## Documentação

A documentação da primeira etapa está disponível na pasta
`documentacao/`.

## Observação

O projeto utiliza somente dados fictícios e informações coletivas.
Não serão armazenados dados clínicos ou informações sensíveis individuais
de estudantes.

# PSE em Ação – Sistema de Planejamento e Acompanhamento de Ações de Saúde na Escola

## 1. Sobre o projeto

O **PSE em Ação** é um sistema desenvolvido em linguagem C como parte da Atividade de Estudo Programado (AEP) do curso de Análise e Desenvolvimento de Sistemas da Universidade Cesumar – Unicesumar.

O objetivo do projeto é auxiliar equipes escolares e profissionais de saúde no planejamento, cadastro e acompanhamento de ações coletivas relacionadas ao Programa Saúde na Escola (PSE).

O sistema funciona por meio de um terminal e permite registrar informações, consultar ações cadastradas, atualizar situações e gerar um resumo geral dos resultados.

## 2. Tecnologias utilizadas

- Linguagem de programação: C.
- Bibliotecas: `stdio.h`, `stdlib.h`, `string.h` e `ctype.h`.
- Estruturas de dados: `struct` e vetores.
- Ambiente de execução: terminal ou prompt de comando.
- Compilador recomendado: GCC.

## 3. Funcionalidades do sistema

O sistema apresenta as seguintes funcionalidades:

| Opção | Funcionalidade | Descrição |
|---|---|---|
| 1 | Cadastrar ação | Permite registrar uma nova ação de saúde. |
| 2 | Listar ações | Exibe todas as ações cadastradas. |
| 3 | Pesquisar ações | Permite pesquisar por código, escola ou tema. |
| 4 | Atualizar situação | Altera a situação de uma ação cadastrada. |
| 5 | Gerar resumo | Apresenta informações e estatísticas gerais. |
| 0 | Sair | Encerra a execução do programa. |

## 4. Como instalar e executar

### 4.1. Pré-requisitos

Para executar o programa, é necessário possuir um computador com um compilador de linguagem C instalado.

Recomenda-se utilizar o GCC ou um ambiente de desenvolvimento que ofereça suporte à linguagem C, como o Dev-C++.

### 4.2. Baixar o projeto

1. Acesse o repositório do projeto no GitHub.
2. Clique no botão **Code**.
3. Selecione **Download ZIP**.
4. Extraia os arquivos para uma pasta do computador.
5. Localize o arquivo-fonte do programa, com extensão `.c`.

### 4.3. Compilar o programa

Caso esteja utilizando o GCC, abra o terminal na pasta onde está localizado o código-fonte e execute:

```bash
gcc pse_em_acao.c -o pse_em_acao
```

Esse comando compila o código-fonte e gera um arquivo executável.

### 4.4. Executar o programa

**No Windows:**

```bash
pse_em_acao.exe
```

**No Linux:**

```bash
./pse_em_acao
```

Após a execução, o menu principal será apresentado no terminal.

## 5. Manual de utilização

### 5.1. Menu principal

Ao iniciar o programa, será exibido o seguinte menu:

```text
================================
       SISTEMA DE ACOES
================================

1 - Cadastrar acao
2 - Listar acoes
3 - Pesquisar acoes
4 - Atualizar situacao
5 - Gerar resumo
0 - Sair

================================
Escolha uma opcao:
```

O usuário deverá digitar o número correspondente à operação desejada.

### 5.2. Cadastrar ação

Ao selecionar a opção 1, o sistema solicitará as seguintes informações:

- Código da ação;
- Escola;
- Tema;
- Data prevista;
- Público-alvo;
- Responsável;
- Quantidade prevista de participantes;
- Situação da ação.

As situações disponíveis são:

- Planejada;
- Realizada;
- Cancelada.

Caso a situação informada seja "realizada", o sistema também solicitará a quantidade efetiva de participantes.

Após o preenchimento das informações, o registro será armazenado e uma mensagem de confirmação será apresentada.

### 5.3. Listar ações

Ao selecionar a opção 2, o sistema apresentará todas as ações cadastradas, exibindo seus respectivos códigos, escolas, temas, datas, públicos-alvo, responsáveis, quantidades previstas e situações.

Quando a ação estiver marcada como realizada, também será apresentada a quantidade efetiva de participantes.

Caso não existam registros, o sistema informará que nenhuma ação foi cadastrada.

### 5.4. Pesquisar ações

Ao selecionar a opção 3, o usuário poderá escolher entre três critérios de pesquisa:

1. Pesquisar por código;
2. Pesquisar por escola;
3. Pesquisar por tema.

Após selecionar o critério, deverá informar o termo desejado.

A pesquisa por escola e tema permite localizar registros que contenham o texto informado, independentemente de letras maiúsculas ou minúsculas.

Caso nenhum registro corresponda à pesquisa, o sistema exibirá uma mensagem informando que nenhuma ação foi encontrada.

### 5.5. Atualizar situação

Ao selecionar a opção 4, o sistema solicitará o código da ação que deverá ser atualizada.

Após localizar o registro, apresentará a situação atual e solicitará a nova situação.

As opções disponíveis são:

- Planejada;
- Realizada;
- Cancelada.

Caso a nova situação seja "realizada", o sistema também solicitará a quantidade efetiva de participantes.

Se o código informado não estiver cadastrado, será apresentada uma mensagem de registro inexistente.

### 5.6. Gerar resumo

Ao selecionar a opção 5, o sistema apresentará um resumo geral das ações cadastradas, contendo:

- Total de ações planejadas;
- Total de ações realizadas;
- Total de ações canceladas;
- Total de participantes previstos;
- Total de participantes efetivos;
- Percentual de participação.

O percentual é calculado considerando a quantidade efetiva de participantes em relação à quantidade total prevista.

## 6. Validações e tratamento de erros

O sistema possui mecanismos para evitar inconsistências durante a utilização.

Entre as validações implementadas estão:

- Impedimento de cadastro com código vazio;
- Impedimento de códigos duplicados;
- Validação de entradas numéricas;
- Impedimento de quantidades negativas de participantes;
- Validação das situações disponíveis;
- Verificação de registros inexistentes durante a atualização;
- Verificação do limite máximo de armazenamento.

O sistema permite armazenar até **100 ações** durante sua execução.

## 7. Armazenamento das informações

Os registros são armazenados em um vetor de estruturas (`struct`) na memória do programa.

As informações permanecem disponíveis enquanto o sistema estiver em execução.

**Importante:** o programa não utiliza banco de dados nem arquivos externos para armazenar os registros. Portanto, ao encerrar a execução, as informações cadastradas são perdidas.

## 8. Limitações do sistema

O PSE em Ação foi desenvolvido com finalidade acadêmica e possui algumas limitações:

- Não possui interface gráfica;
- Não utiliza banco de dados;
- Não mantém os registros após o encerramento;
- Permite o armazenamento de até 100 ações por execução;
- Não possui cadastro individual de estudantes;
- Não armazena informações clínicas ou dados pessoais sensíveis.

O sistema é destinado exclusivamente à organização de informações coletivas relacionadas às ações de saúde na escola.

## 9. Considerações finais

O desenvolvimento do PSE em Ação possibilitou aplicar conhecimentos de lógica de programação, estruturas condicionais, funções, vetores, estruturas de repetição e manipulação de dados em linguagem C.

A implementação das funcionalidades permite organizar e acompanhar ações coletivas do Programa Saúde na Escola, facilitando a consulta das informações e a visualização dos resultados.

Apesar das limitações relacionadas ao armazenamento em memória e à ausência de uma interface gráfica, o projeto demonstra como a programação pode contribuir para solucionar problemas de organização e gerenciamento de informações.

Como possibilidades de melhoria, destacam-se a implementação de banco de dados, armazenamento permanente, interface gráfica e geração de relatórios mais detalhados.

---

**Projeto acadêmico – AEP 2026**

Universidade Cesumar – Unicesumar  
Curso: Análise e Desenvolvimento de Sistemas  
Projeto: PSE em Ação
