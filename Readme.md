# Desafio Versão_2
## Otimizando o Sistema Bancário com Funções Python
## Este desafio faz parte da atividade do **Bootcamp - Suzano - Python Developer** que estou realizando na plataforma da [DIO (Digital Innovation One)](https://www.dio.me/), em parceria com a empresa [SUZANO](https://www.suzano.com.br).

### Objetivo Geral

Separar as funções existentes de saque, depósito e extrato em funções. Criar duas novas funções: cadastrar usuário (cliente) e cadastrar conta bancária.

### Desafio

Precisamos deixar nosso código mais modularizado, para isso vamos criar funções para as operações existentes: sacar, depositar e visualizar histórico. Além disso, para a versão 2 do nosso sistema, precisamos criar duas novas funções: criar usuário (cliente do banco) e criar conta corrente (vincular com usuário).

### Separação em funções

Devemos criar funções para todas as operações do sistema.
Para exercitar tudo o que aprendemos neste módulo, cada função vai ter uma regra na passagem de argumentos. O retorno e a forma como serão chamadas, podem ser definidas por você da forma que achar melhor.

### Funções

#### 1. **Saque**
A função saque deve receber os argumentos apenas por nome (keyword only).  
**Sugestão de argumentos**: `saldo`, `valor`, `extrato`, `limite`, `numero_saques`, `limite_saques`.  
**Sugestão de retorno**: `saldo` e `extrato`.

#### 2. **Depósito**
A função depósito deve receber os argumentos apenas por posição (positional only).  
**Sugestão de argumentos**: `saldo`, `valor`, `extrato`.  
**Sugestão de retorno**: `saldo` e `extrato`.

#### 3. **Extrato**
A função extrato deve receber os argumentos por posição e nome (positional only e keyword only).  
**Argumentos posicionais**: `saldo`, **argumentos nomeados**: `extrato`.

### Novas funções

Precisamos criar duas novas funções: **criar usuário** e **criar conta corrente**. Fique à vontade para adicionar mais funções, exemplo: listar contas, listar usuários, inativar conta.

#### 1. **Criar usuário (cliente)**
O Programa deve armazenar os usuários em uma lista.  
Um usuário é composto por: `nome`, `data de nascimento`, `cpf` e `endereço`.  
O `endereço` é uma string com o formato: `logradouro, nro - bairro - cidade/sigla estado`.  
Deve ser armazenado somente os números do CPF. Não podemos cadastrar 2 usuários com o mesmo CPF.

#### 2. **Criar conta corrente**
O programa deve armazenar contas em uma lista.  
Uma conta é composta por: `agência`, `número da conta` e `usuário`.  
O número da conta é sequencial, iniciando em 1. O número da agência é fixo: "0001".  
O usuário pode ter mais de uma conta, mas uma conta pertence somente a um usuário.

#### 3. **Filtrar usuário**
O programa deve permitir a filtragem de usuários cadastrados, buscando um usuário específico com base no CPF. A função responsável por isso verifica se o CPF informado já está registrado e retorna o usuário correspondente, caso encontrado.

#### 4. **Listar contas**
O programa deve exibir todas as contas criadas, mostrando informações como: número da agência, número da conta e o nome do titular da conta. Isso facilita o acompanhamento das contas ativas e vinculadas a cada usuário.

### Dica

Para vincular um usuário a uma conta, filtre a lista de usuários buscando o número do CPF informado para cada usuário da lista.

## Conclusão

Este desafio foi uma excelente oportunidade para aprimorar minhas habilidades em Python, especialmente na modularização de código e na manipulação de estruturas de dados como listas e dicionários. Aprendi a criar funções específicas para cada operação do sistema bancário, garantindo um código mais organizado, reutilizável e de fácil manutenção. Além disso, a implementação das novas funcionalidades, como cadastro de usuários e contas, me permitiu explorar conceitos importantes como validação de dados e relacionamento entre entidades.

Agradeço à [DIO](https://www.dio.me/) e à [SUZANO](https://www.suzano.com.br) por proporcionarem essa experiência enriquecedora no Bootcamp. Estou animada para continuar aprendendo e aplicando esses conhecimentos em projetos futuros!

---

**Autor**: Raiane Batista  
**Data**: 11-02-2025  
**Bootcamp**: Python Developer - Suzano  
**Plataforma**: [DIO](https://www.dio.me/)
