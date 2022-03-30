# Meu Primeiro Git

Repositório para praticar git e gitflow.

## Comandos

Principais comandos do GIT

### Branches

Para criar uma branch, use `git checkout - b prefixo/nome-da-branch`

Para mudar de branch, use `git checkout prefixo/nome-da-branch`

Para listar as branches, use `git branch`

E para apagar uma branch, use `git branch prefixo/nome-da-branch -D`

### Atualizações

Para adicionar uma atualização, use `git add .`, onde `.` representa a pasta onde está atualmente (no terminal). Você pode adicionar tudo o que estiver na pasta (e que foi modificado) ou pode adicionar arquivos ou pastas específicas (`git add ./index.html`).

Para comitar as alterações adicionadas, devemos executar `git commit -m 'prefixo: descrição do commit` - importante que a descrição seja clara para facilitar futuras buscas no repositório, seja para achar uma funcionalidade ou um motivo de bug.

Para "empurrar" as atualizações para a origem, rode `git push origin prefixo/nome-de-branch`. Se for uma branch que só existe localmente, poderá abrir uma PR.

Para "puxar" as atualizações da origem, rode `git pull origin prefixo/nome-de-branch`.

Para mergear uma PR já aprovada - via terminal - acesse a branch que deve receber a PR/atualizações com `git checkout prefixo/nome-da-branch-que recebe-a-pr`, rode um `git pull prefixo/nome-da-branch-que recebe-a-pr` para garantir que está atualizada, e, por fim, `git merge prefixo/prefixo/nome-da-branch-que recebe-a-pr`. Agora, você tem as alterações localmente. Só falta jogar para a origem (`git push origin prefixo/nome-da-branch-que recebe-a-pr`).
