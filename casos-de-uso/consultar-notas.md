# Caso de Uso: Consultar Notas

## Objetivo
Permitir que o aluno consulte suas notas no sistema escolar.

## Atores
- Aluno

## Pré-condições
- O aluno deve estar cadastrado no sistema.
- O aluno deve estar autenticado.

## Pós-condições
- As notas do aluno são exibidas na tela.

## Diagrama de Caso de Uso

![Diagrama de Caso de Uso](imagens/caso-de-uso-escola.png)

## Fluxo Principal
1. O aluno acessa o sistema escolar.
2. O sistema solicita as credenciais de acesso.
3. O aluno informa login e senha.
4. O sistema valida as credenciais.
5. O aluno seleciona a opção **Consultar notas**.
6. O sistema recupera as notas do aluno.
7. O sistema exibe as notas por disciplina.

## Fluxo Alternativo
### A1. Visualizar boletim
1. Após a exibição das notas, o aluno seleciona a opção **Ver boletim**.
2. O sistema gera a visualização do boletim.
3. O sistema exibe o boletim ao aluno.

## Fluxo de Exceção
### E1. Credenciais inválidas
1. No passo 4 do fluxo principal, o sistema identifica que o login ou a senha estão incorretos.
2. O sistema exibe uma mensagem de erro.
3. O sistema retorna à tela de autenticação.
