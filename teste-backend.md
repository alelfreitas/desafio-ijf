# Teste BACK-END

## Utilize os seguintes frameworks/biblitecas/orms:
- Typescript
- NestJS
- SQL
- Prisma

## A entrega deve ser feita através do github.

## Itens avaliados: 
- funcionamento
- lógica
- design de código
- utilização do framework
- documentação e testes

## A base deve estar em docker dentro do projeto
## O projeto pode estar em docker
## Crie as seeds e migrations da base
## Documente a entrega utilizando arquivos MD com o roteiro de utilização e o que julgar necessário explicar 

Cada um desses itens tem uma pontuação individual, o que significa que mesmo que não consiga realizar todo o desenvolvimento, será considerado o que for entregue.
Inclusão de testes no código melhoram a pontuação na avaliação. 

# Contexto do projeto:

Você foi contratado para desenvolver o back-end de um sistema de cadastramento de cursos online, esse sistema possui dois tipos de acesso:

- Professor (Nome, usuário)
- Aluno (Nome, usuário)

O sistema permite que o PROFESSOR cadastre novos cursos (Nome, descrição, banner).
Apenas o PROFESSOR pode criar, editar ou excluir cursos.
O PROFESSOR pode liberar ou remover acesso para determinados alunos ou todos a algum curso.

O curso é formado por uma ou mais aulas, cada aula pode conter:
Um texto, ou um arquivo (pdf, xlsx, docx, pptx) ou um link.

O professor consegue ver todos os alunos com acesso ao curso e quantas aulas do total eles visualizaram.
O professor pode aprovar um aluno, CONTANTO QUE esse aluno tenha assistido a 100% das aulas daquele curso.

O aluno consegue visualizar os cursos e aulas e somente dos cursos aos quais ele tiver sido cadastrado.
Cada aula que o aluno visualizar é registrada no sistema vinculada ao seu usuário.

O aluno consegue ver seu status no curso:
Não iniciado:  quando tem 0 aulas visualizadas
Em andamento: quando tem ao menos uma aula visualizada
Finalizado: Quando tem 100% das aulas visualizadas, porém sem aprovação do professor
Aprovado: Quando o professor aprova

Um aluno não consegue ver os cursos, aulas, e nem dados de outros alunos. Apenas os próprios.

Considere as **regras de acesso** nas APIS, você pode simular o envio da informação no header e/ou considerar o usuário realizando a requisição.
Não deve ser possível realizar a chamada sem ser um usuário cadastrado.

Detalhe como deve ser feito a chamada simulando cada um dos acessos.

Caso necessário deixe cadastrado ao menos 2 usuários de cada perfil.
Não é obrigatório criar um sistema de login e token, você pode simular o acesso com tokens específicos no header se for o caso. Só não esqueça de mencioná-los na documentação da resposta para realização de testes.
