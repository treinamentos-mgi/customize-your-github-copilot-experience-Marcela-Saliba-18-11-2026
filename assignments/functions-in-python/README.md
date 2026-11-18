# 📘 Atividade: Funções em Python

## 🎯 Objetivo

Aprenda a criar funções em Python para organizar e reutilizar o seu código. Você vai praticar a definição de funções, o uso de parâmetros e o retorno de valores. Ao final, terá um pequeno programa que usa funções para resolver problemas em partes separadas. Você vai conseguir!

## 📝 Tarefas

### 🛠️ Criar a Primeira Função

#### Descrição
Crie um arquivo `funcoes.py` e defina uma função chamada `saudar` que não recebe parâmetros e apenas imprime uma mensagem. Em seguida, chame a função no próprio arquivo para ver o resultado. Uma função é um bloco de código com nome que pode ser executado sempre que você precisar.

#### Requisitos
O programa concluído deve:

- Definir uma função `saudar()` usando a palavra-chave `def`.
- Imprimir a mensagem `Olá, aluno de programação!` quando a função for chamada.
- Chamar `saudar()` pelo menos uma vez no arquivo.

Exemplo de saída:

```text
Olá, aluno de programação!
```

### 🛠️ Funções com Parâmetros e Retorno

#### Descrição
Crie funções que recebem dados por meio de parâmetros e devolvem um resultado com `return`. Parâmetros são valores que você passa para a função entre parênteses. O `return` envia o resultado de volta para quem chamou a função.

#### Requisitos
O programa concluído deve:

- Definir uma função `calcular_media(nota1, nota2, nota3)` que retorna a média das três notas.
- Definir uma função `situacao(media)` que retorna `"Aprovado"` quando a média for maior ou igual a 6 e `"Reprovado"` caso contrário.
- Exibir a média com duas casas decimais e a situação do aluno a partir das duas funções.

Exemplo de entrada e saída:

```text
Entrada: 7, 8, 9
Saída:   Média: 8.00 - Aprovado
```

### 🛠️ Organizar um Programa com Funções

#### Descrição
Organize um programa maior dividindo o problema em funções menores. Você vai criar uma função que recebe uma lista de notas de vários alunos, calcula a média de cada um e mostra o resultado. Cada função deve ter uma única responsabilidade.

#### Requisitos
O programa concluído deve:

- Usar as funções `calcular_media` e `situacao` da tarefa anterior, sem repetir o código delas.
- Definir uma função `processar_alunos(alunos)` que recebe um dicionário, em que a chave é o nome do aluno e o valor é a lista de três notas.
- Para cada aluno, exibir o nome, a média com duas casas decimais e a situação.
- Definir uma função `contar_aprovados(alunos)` que retorna quantos alunos foram aprovados.

Exemplo de entrada e saída:

```text
Entrada: {"Ana": [7, 8, 9], "Bruno": [4, 5, 6]}
Saída:
Ana: média 8.00 - Aprovado
Bruno: média 5.00 - Reprovado
Aprovados: 1
```
