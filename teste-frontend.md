# Teste FRONT-END

## Utilize os seguintes frameworks/biblitecas

- Typescript
- Next.js
- React.js
- MUI ou Ant

## A entrega deve ser feita através do github.

## Itens avaliados: 
- funcionamento
- lógica
- design de código
- utilização do framework
- documentação e testes

```
As requisições podem ser feitas utilizando json simulando a resposta do backend
O projeto deve estar em docker, configurado de forma que o resultado do build seja exposto no servidor web (utilize SSR e não estático)
Utilização de turborepo será considerado um diferencial
Documente a entrega utilizando arquivos MD com o roteiro de utilização e o que julgar necessário explicar 
```

# Contexto do projeto:

Você foi contratado para desenvolver o front-end de um sistema de cadastramento de cursos online, esse sistema possui dois acessos:

- Professor (Quem registra os cursos e da acesso para os alunos aos cursos)
- Aluno (Quem visualiza os cursos que possui acesso)

O sistema permite que o PROFESSOR cadastre novos cursos (Nome, descrição, banner).
Apenas o PROFESSOR vizualizar as telas de criação de curso.
O PROFESSOR pode liberar ou remover acesso para determinados alunos ou todos a algum curso.

O curso é formado por uma ou mais aulas, cada aula pode conter:
Um texto, ou um arquivo ou um link.

O professor consegue ver todos os alunos com acesso ao curso e quantas aulas do total eles visualizaram.
O professor pode aprovar um aluno.

O aluno consegue visualizar os cursos e aulas.
Cada aula que o aluno visualizar envia para o backend uma requisição para informar que ele visualizou aquela aula.

O aluno consegue ver seu status no curso (conforme a informação que vem do backend):
Não iniciado:  quando tem 0 aulas visualizadas
Em andamento: quando tem ao menos uma aula visualizada
Finalizado: Quando tem 100% das aulas visualizadas, porém sem aprovação do professor
Aprovado: Quando o professor aprova

Um aluno não consegue ver os cursos, aulas, e nem dados de outros alunos. Apenas os próprios.

As regras de acesso são capturadas pelo backend através do token enviado no header junto da requisição.

Não é obrigatório criar um sistema de login e token, você pode simular o acesso com tokens específicos no header se for o caso. Só não esqueça de mencioná-los na documentação.
