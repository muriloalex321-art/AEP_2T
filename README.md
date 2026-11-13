# PSE em Ação
## Sistema de Planejamento e Acompanhamento de Ações de Saúde na Escola

Projeto acadêmico desenvolvido em linguagem C como parte da Atividade de Estudo Programado (AEP) do curso de Análise e Desenvolvimento de Sistemas da Universidade Cesumar – UNICESUMAR.

## Integrantes
- Murilo Alexandre de Assis — RA 26010057-2
- Arthur Mingroni Pacheco — RA 26006047-2
- Joelson Batista dos Santos — RA 26012817-2

## Objetivo
Apoiar o planejamento e o acompanhamento de ações coletivas relacionadas ao Programa Saúde na Escola (PSE), permitindo registrar ações, consultar informações, atualizar situações e visualizar indicadores quantitativos.

## Funcionalidades
| Opção | Funcionalidade |
|---|---|
| 1 | Cadastrar ação |
| 2 | Listar ações |
| 3 | Pesquisar por código, escola ou tema |
| 4 | Atualizar situação e participantes efetivos |
| 5 | Gerar resumo quantitativo |
| 0 | Encerrar |

## Requisitos
- Sistema operacional Windows, Linux ou equivalente.
- Compilador C, preferencialmente GCC.
- Terminal ou prompt de comando.

## Como obter e executar
1. No GitHub, clique em **Code > Download ZIP** e extraia o conteúdo.
2. Abra o terminal na pasta em que está o arquivo-fonte `.c`.
3. Compile com GCC. Se o arquivo se chamar `sistema.c`, use:

```bash
gcc -std=c11 -Wall -Wextra -pedantic sistema.c -o sistema
```

4. Execute:
   - Windows: `sistema.exe`
   - Linux: `./sistema`

> Se o arquivo tiver outro nome, substitua `sistema.c` pelo nome real do arquivo e ajuste também o nome do executável.

## Dados e armazenamento
Os registros são armazenados em um vetor com capacidade máxima de 100 ações. Os dados permanecem disponíveis somente durante a execução do programa e são perdidos quando ele é encerrado. Esta versão não utiliza banco de dados nem gravação permanente em arquivos.

## Testes
Foi realizada compilação com GCC utilizando `-std=c11 -Wall -Wextra -pedantic` e execução automatizada de 13 cenários funcionais sobre uma reprodução do código-fonte fornecido para a documentação: **13 aprovados e 0 reprovados**. Para registrar a validação final do repositório, recomenda-se executar os mesmos cenários diretamente sobre o arquivo `.c` publicado no GitHub.

Os cenários verificaram listagem vazia, cadastro, código vazio e duplicado, quantidades negativas, situação inválida, pesquisa, atualização, cálculo do percentual, total previsto zero, limite de 100 registros, opção inválida e encerramento.

## Documentação
- Documento final do projeto: `Documento_Final_PSE_em_Acao.docx`
- Manual do usuário: `Manual_do_Usuario_PSE_em_Acao.docx`
- Relatório de testes: `Relatorio_de_Testes_PSE_em_Acao.txt`
- Fluxograma: `Fluxogramas.png` (se incluído no repositório)

## Vídeo de apresentação
https://youtu.be/eHTGGpONv-M?si=nMPXc1_BId-cgqSD

## Observação
O projeto utiliza informações coletivas e fictícias. Não deve ser utilizado para armazenar dados clínicos ou dados pessoais sensíveis de estudantes.
