# Guia de Referência para Criar Tarefas

Use este guia ao definir o escopo, a dificuldade e os materiais de uma nova assignment.

## 1. Objetivos de Aprendizado

Antes de escrever a tarefa, defina de 1 a 3 objetivos de aprendizado claros. Cada objetivo deve descrever algo que o aluno conseguirá fazer ao final, por exemplo:

- "Usar `for` para percorrer listas"
- "Criar funções que recebem parâmetros e retornam valores"

Todas as tarefas geradas devem refletir esses objetivos na seção `## 🎯 Objetivo`.

## 2. Nível de Dificuldade

Escolha o nível de acordo com os conceitos que os alunos já conhecem:

| Nível | Perfil do aluno | Exemplo de tarefa |
|-------|-----------------|-------------------|
| Iniciante | Primeiro contato com programação | Calcular a média de três notas |
| Intermediário | Já usa variáveis, condicionais e laços | Contar palavras em um arquivo de texto |
| Avançado | Domina funções, listas e estruturas de dados | Implementar um jogo com regras e pontuação |

Quando houver dúvida, escolha o nível inferior. É melhor que o aluno conclua a tarefa com confiança do que desista logo no início.

## 3. Escopo

- Limite a tarefa a um ou dois conceitos principais.
- Prefira tarefas que possam ser concluídas em uma a duas aulas.
- Divida problemas grandes em tarefas menores (`### 🛠️ ...`), cada uma com um resultado verificável.
- Evite dependências externas, a menos que sejam essenciais ao conceito ensinado.

## 4. Quando Incluir Starter Code

Inclua arquivos iniciais (starter code) quando:

- A tarefa depender de uma estrutura básica que não é o foco do aprendizado (por exemplo, leitura de arquivo ou interface do jogo).
- O aluno precisar começar de um ponto específico para evitar erros de configuração.

Não inclua starter code quando o objetivo for justamente criar a estrutura do programa, como definir funções ou organizar um laço do zero.

Ao adicionar starter code, registre-o como attachment com o tipo adequado (`python`, `csv`, `json`, `txt`, `html`).

## 5. Linguagem e Tom

- Escreva em português claro e direto.
- Use um tom encorajador, como "Você vai conseguir", sem exagerar.
- Explique termos técnicos na primeira vez em que aparecerem.
- Nos requisitos, descreva resultados mensuráveis, por exemplo: "O programa exibe a média com duas casas decimais".

## 6. Exemplos de Entrada e Saída

Inclua exemplos em blocos de código quando ajudarem a esclarecer o resultado esperado:

```text
Entrada: 7, 8, 9
Saída: Média: 8.00
```

## 7. Checklist Final

- [ ] Os objetivos de aprendizado estão claros
- [ ] A dificuldade corresponde ao nível dos alunos
- [ ] A tarefa cobre um ou dois conceitos principais
- [ ] Os requisitos são específicos e verificáveis
- [ ] O starter code foi incluído apenas quando necessário
- [ ] A estrutura segue o [template de assignment](../../../../templates/assignment-template.md)
