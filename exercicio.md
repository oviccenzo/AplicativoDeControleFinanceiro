Estudo de Caso — Aplicativo de Controle
Financeiro
Disciplina: Programação para Dispositivos Móveis
Projeto: Meu Controle Financeiro

## 1. Contextualização
O controle das finanças pessoais é uma atividade importante para compreender como o dinheiro é recebido e utilizado no dia a dia. Entretanto, muitas pessoas ainda utilizam anotações em papel, planilhas ou simplesmente tentam memorizar suas despesas e receitas. 

Diante desse cenário, você foi convidado(a) a desenvolver um aplicativo para dispositivos móveis que permita ao usuário registrar e acompanhar suas movimentações financeiras.

O aplicativo deverá possibilitar o cadastro de receitas e despesas, permitindo que o usuário consulte suas movimentações e acompanhe automaticamente o seu saldo financeiro.

Este projeto tem como objetivo dar continuidade aos conhecimentos desenvolvidos durante a implementação do aplicativo de lista telefônica, especialmente os conceitos de:

• criação de telas
• componentes de interface
• entrada de dados
• validação de informações
• listas
• navegação entre telas
• cadastro de registros
• edição de registros
• exclusão de registros
• organização e apresentação de informações

Além desses conceitos, o novo projeto deverá introduzir situações relacionadas a cálculos, categorias, datas, filtros e resumo de informações.

## 2. Objetivo do projeto
Desenvolver um aplicativo móvel denominado Meu Controle Financeiro, capaz de registrar e consultar receitas e despesas pessoais e apresentar automaticamente um resumo financeiro do usuário.

Ao final do projeto, o aplicativo deverá permitir que o usuário responda, de forma simples, perguntas como:

• Quanto eu recebi?
• Quanto eu gastei?
• Qual é o meu saldo?
• Com o que estou gastando?
• Quais movimentações foram registradas?
• Quais são minhas despesas de determinada categoria?

## 3. Funcionalidades obrigatórias
3.1 Cadastro de movimentação
O usuário deverá conseguir cadastrar uma nova movimentação financeira.
Campo      Nome ou identificação da movimentação  
Descrição  Valor financeiro da movimentação
Valor      Receita ou Despesa
Tipo       Categoria à qual a movimentação pertence
Categoria  Data em que a movimentação ocorreu

Exemplos de movimentações
Receitas: Salário — R$ 2.500,00; Freelance — R$ 500,00; Venda de produto — R$ 150,00.

Despesas: Supermercado — R$ 350,00; Combustível — R$ 150,00; Cinema — R$ 50,00; Conta de telefone — R$ 80,00.

## 4. Tipos de movimentação
Receita

Representa um valor que entrou para o usuário. Exemplos: salário; pagamento recebido; freelance; venda; outros recebimentos.

Despesa
Representa um valor que saiu do usuário. Exemplos: alimentação; transporte; aluguel; lazer; contas; compras.

O tipo deverá ser selecionado pelo usuário durante o cadastro.

## 5. Categorias
Cada movimentação deverá estar associada a uma categoria.

O aplicativo deverá disponibilizar, no mínimo:

• Alimentação
• Transporte
• Moradia
• Saúde
• Educação
• Lazer
• Salário
• Outros

O aluno poderá acrescentar outras categorias caso considere necessário.

## 6. Tela principal
A tela principal deverá apresentar um resumo das informações financeiras e a lista de movimentações cadastradas. 

----------------------------------
MEU CONTROLE FINANCEIRO
----------------------------------

Receitas

R$ 2.500,00

Despesas

R$ 580,00

Saldo

R$ 1.920,00
----------------------------------

MOVIMENTAÇÕES

20/09 Salário
Receita R$ 2.500,00

20/09 Supermercado
Despesa R$ 350,00

21/09 Combustível
Despesa R$ 150,00
----------------------------------
[+ Nova movimentação]

A aparência poderá ser diferente desse exemplo. O objetivo é apenas demonstrar uma
possível organização das informações.

## 7. Resumo financeiro
Total de receitas: soma de todas as movimentações classificadas como Receita.

Total de despesas: soma de todas as movimentações classificadas como Despesa.

Saldo: Saldo = Total de Receitas − Total de Despesas.

Exemplo: Salário R$ 2.500,00; Supermercado R$ 300,00; Combustível R$ 150,00; Cinema R$ 50,00.

Receitas: R$ 2.500,00
Despesas: R$ 500,00
Saldo: R$ 2.000,00

Esses valores deverão ser atualizados automaticamente sempre que uma movimentação for cadastrada, alterada ou excluída.

## 8. Cadastro de movimentação
Ao selecionar a opção "Nova movimentação", o aplicativo deverá apresentar um formulário.

Descrição: campo de texto para informar a descrição. Exemplo: Supermercado.

Valor: campo para informar o valor da movimentação. Exemplo: 350,00.

Tipo: o usuário deverá escolher entre Receita e Despesa.
( ) Receita
( ) Despesa

Categoria: o usuário deverá selecionar uma das categorias disponíveis.
[ Alimentação ▼ ]

Data: o usuário deverá informar ou selecionar a data da movimentação.

Botões:
[ Salvar ] [ Cancelar ]

## 9. Validação dos dados
O aplicativo deverá realizar validações antes de salvar uma movimentação.
Regra 1 — Descrição obrigatória 
Não será permitido cadastrar uma movimentação sem descrição. Mensagem sugerida: "Informe a descrição da movimentação."

Regra 2 — Valor obrigatório
Não será permitido cadastrar uma movimentação sem informar o valor. Mensagem sugerida: "Informe o valor da movimentação."

Regra 3 — Valor positivo
O valor deverá ser maior que zero. Não deverão ser aceitos valores negativos.

Regra 4 — Tipo obrigatório
O usuário deverá selecionar se a movimentação é uma receita ou despesa.

Regra 5 — Categoria obrigatória
O usuário deverá selecionar uma categoria.

Regra 6 — Data obrigatória
O usuário deverá informar a data da movimentação.

## 10. Visualização das movimentações
As movimentações cadastradas deverão ser apresentadas em uma lista. Cada item deverá apresentar, no mínimo: descrição; valor; tipo; categoria; data.----------------------------------
Supermercado
Alimentação
21/09/2026
Despesa
R$ 350,00
----------------------------------
Salário
Salário
20/09/2026
Receita
R$ 2.500,00
----------------------------------
A organização visual fica a critério do aluno.

## 11. Visualização dos detalhes
Ao selecionar uma movimentação na lista, o aplicativo deverá apresentar uma tela contendo todos os seus dados.
DETALHES DA MOVIMENTAÇÃO

Descrição:
Supermercado

Valor:
R$ 350,00

Tipo:
Despesa

Categoria:
Alimentação

Data:
21/09/2026

[ Editar ] [ Excluir ]

## 12. Edição de movimentação
O usuário deverá conseguir alterar uma movimentação cadastrada. Ao selecionar "Editar", o aplicativo deverá abrir o formulário preenchido com os dados atuais.

Descrição:
Supermercado

Valor:
350,00

Tipo:
Despesa

Categoria:
Alimentação

Data:
21/09/2026
O usuário poderá modificar qualquer informação e salvar novamente. Após a alteração, o resumo financeiro deverá ser atualizado.

## 13. Exclusão de movimentação
O usuário deverá conseguir excluir uma movimentação. Antes da exclusão definitiva, o aplicativo deverá apresentar uma mensagem de confirmação.

Deseja realmente excluir esta movimentação?
[ CANCELAR ] [ EXCLUIR ]

Caso o usuário escolha Cancelar, a movimentação deverá permanecer cadastrada. Caso escolha Excluir, a movimentação deverá ser removida e os valores do resumo financeiro deverão ser recalculados.

## 14. Filtro de movimentações
Além das funcionalidades básicas de cadastro, edição e exclusão, o aplicativo deverá permitir que o usuário filtre as movimentações.

Todas
Receitas
Despesas

Ao selecionar Despesas, a lista deverá apresentar somente as movimentações classificadas como despesas. Ao selecionar Receitas, deverão aparecer somente as receitas. Ao selecionar Todas, todas as movimentações deverão ser apresentadas novamente.

## 15. Desafio adicional — filtro por categoria
Como atividade de extensão, o aluno poderá implementar um filtro por categoria.
Categoria:
[ Todas ▼ ]
[ Alimentação ]
[ Transporte ]
[ Moradia ]
[ Saúde ]
[ Educação ]
[ Lazer ]
[ Salário ]
[ Outros ]
Ao selecionar Alimentação, por exemplo, deverão ser exibidas somente as movimentações dessa categoria.

## 16. Desafio adicional — pesquisa
Como segundo desafio, o aplicativo poderá disponibilizar uma caixa de pesquisa.
 Pesquisar movimentação
[ supermercado ]
O aplicativo deverá apresentar as movimentações cuja descrição corresponda ao texto pesquisado. Por exemplo, se o usuário pesquisar super, poderá encontrar: Supermercado; Supermercado do bairro; Compra supermercado.

## 17. Persistência dos dados
Os dados cadastrados deverão permanecer disponíveis de acordo com o mecanismo de
armazenamento trabalhado na disciplina.

Caso a disciplina ainda não tenha abordado banco de dados ou armazenamento local, o professor poderá permitir inicialmente que os alunos trabalhem apenas com os dados em memória.

Como evolução do projeto, o aplicativo deverá armazenar as movimentações localmente para que elas não sejam perdidas quando o aplicativo for encerrado.

## 18. Requisitos mínimos da interface
• os campos deverão possuir identificação clara;
• os botões deverão indicar claramente sua função;
• os valores financeiros deverão ser apresentados de maneira adequada;
• o usuário deverá conseguir navegar entre as telas de forma intuitiva;
• mensagens de erro deverão ser claras;
• operações de exclusão deverão solicitar confirmação.
Não é necessário desenvolver uma interface visualmente complexa. O foco principal da atividade é a implementação das funcionalidades.

## 19. Telas esperadas
Tela 1 — Principal: total de receitas; total de despesas; saldo; lista de movimentações; opção para cadastrar uma nova movimentação; opção de filtro.

Tela 2 — Cadastro: informar descrição; informar valor; selecionar tipo; selecionar categoria; informar data; salvar ou cancelar.

Tela 3 — Detalhes: apresentar os dados completos de uma movimentação e permitir editar e excluir.

Tela 4 — Edição: permitir alterar os dados de uma movimentação existente.
A implementação poderá utilizar telas diferentes dessas, desde que todas as funcionalidades solicitadas estejam disponíveis.

## 20. Situação-problema
Considere a seguinte situação:
João recebe seu salário mensalmente e deseja utilizar o aplicativo para controlar seus gastos.

No dia 20/09, João recebeu: Salário — R$ 2.500,00.

No mesmo dia, registrou: Supermercado — R$ 300,00.

No dia 21/09, registrou: Combustível — R$ 150,00.

E no dia 22/09: Cinema — R$ 50,00.

Após cadastrar essas movimentações, o aplicativo deverá apresentar:

Total de receitas: R$ 2.500,00

Total de despesas: R$ 500,00

Saldo: R$ 2.000,00

Posteriormente, João percebe que o gasto com combustível foi de R$ 180,00, e não R$ 150,00. Ele

deverá conseguir editar a movimentação.

Após a alteração, o aplicativo deverá recalcular automaticamente:

Total de receitas: R$ 2.500,00

Total de despesas: R$ 530,00

Saldo: R$ 1.970,00

## 21. Requisitos técnicos
O projeto deverá ser desenvolvido utilizando as tecnologias e ferramentas apresentadas durante a disciplina.

O aluno deverá demonstrar a utilização dos conceitos estudados em aula, tais como:

• componentes de interface 
• eventos de interação
• navegação
• gerenciamento de estado
• listas
• formulários
• validação
• manipulação de dados
• operações de inclusão
• operações de alteração
• operações de exclusão
• cálculos
O uso de bibliotecas ou recursos adicionais deverá ser justificado quando solicitado pelo professor.

## 22. Entrega
O aluno deverá entregar:

• Código-fonte do aplicativo;

• Aplicativo funcionando em emulador ou dispositivo físico;

• Breve documentação, contendo: nome do aplicativo; descrição da solução; tecnologias utilizadas; descrição das telas; principais funcionalidades;

• Capturas de tela das principais funcionalidades.
