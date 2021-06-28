# Sistema Bancário

Você e sua equipe foram contratados para realizar a implementação de um sistema bancário
usando a linguagem Python versão 3. O sistema deverá ser executado via linha de comando
e os dados deverão ser armazenados toda vez que o sistema for fechado. Para armazenar os
dados, sugere-se utilizar o pacote pickle.
O sistema deverá possuir duas interfaces, sendo que cada uma deverá ser implementada em
um arquivo Python diferente:
1. Interface de gerente
2. Interface de cliente

Cada uma destas interfaces apresentará ao seu usuário um conjunto diferente de
funcionalidades que são descritas abaixo.

INTERFACE DO GERENTE

A interface do gerente permitirá ao gerente do banco cadastrar novas contas, buscar uma
conta existente, ou definir a nova senha de uma conta existente.
- Cadastro de nova conta: O sistema requisitará ao gerente o nome completo do cliente, sua
profissão, renda mensal, endereço e telefone. O número da conta corrente deverá possuir 5
dígitos e deverá ser do tipo inteiro.
- Busca de conta corrente: O sistema requisitará ao gerente o nome de um cliente e listará
todas as contas cujo nome informado esteja incluído no nome cadastrado na base de dados.
- Definição de nova senha: O sistema requisitará o número de uma conta corrente e verificará
se a conta existe. Se a conta existir, o sistema requisitará uma nova senha, que deverá possuir
entre 4 a 8 caracteres alfanuméricos. O sistema deverá recusar senhas com acentos e/ou
caracteres especiais.

INTERFACE DO CLIENTE

A interface do cliente permitirá ao mesmo realizar diversas operações visando movimentação
de dinheiro.
- Saque: O cliente fornecerá sua conta corrente e senha. Caso os valores estejam corretos, o
cliente fornecerá o valor a ser sacado de sua conta corrente. Este valor deverá ser maior que
R$0,00 (zero) e também não poderá ser maior que o saldo atual da conta corrente. O sistema
deverá questionar se todos os dados estão corretos antes de efetuar a dedução na conta
corrente.
- Depósito: O cliente fornecerá sua conta corrente e senha. Caso os valores estejam corretos,
o cliente fornecerá o valor a ser depositado em sua conta corrente. O valor fornecido deverá
ser maior que R$0,00 (zero) e deverá ser de no máximo R$10.000,00 (dez mil reais). O sistema 
deverá questionar se todos os dados estão corretos antes de efetuar o depósito na conta
corrente.
- Visualização de saldo: O cliente fornecerá sua conta corrente e senha. Caso os dados
estejam corretos, o sistema deverá apresentar o nome completo do cliente, sua conta
corrente e saldo.
- Simulação de investimento: O cliente deverá fornecer o número de meses do investimento,
assim como o valor do aporte inicial. Para este investimento, deve-se assumir que o
rendimento será de 1,5% ao mês e que o montante é calculado usando juros compostos.
Ainda, assume-se que o banco possui uma taxa de administração de 1% ao ano. Caso o
investimento seja feito por um intervalo menor que 1 ano, deve-se assumir 1% de taxa de
administração, e caso o investimento seja realizado por mais que 5 anos, então a taxa de
administração anual é de 0,5%.
