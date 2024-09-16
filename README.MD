# Action para criação de pull request de forma automática
Esta action visa facilidade no que diz respeito a criação de pull request de forma automática de uma branch, (feature/**), para a branch main

## Como usar?
Para que esta action funcione corretamente em seu repositório, é preciso a criação de um personal access token com permições específicas para a criação do pull request, já que o token padrão fornecido pelo Github não tem essas permições

### 1. Gerar um Personal Access Token (PAT)
1. Vá para a [página de tokens do GitHub](https://github.com/settings/tokens).
2. Clique no botão "Generate new token".
3. Dê um nome para o token (ex: "GitHub Actions Token").
4. Selecione as permissões necessárias:
   - **repo**: Acesso completo a repositórios públicos e privados.
   - **workflow**: Acesso a workflows do GitHub Actions.
5. Clique em "Generate token".
6. Copie o token gerado (guarde-o em um lugar seguro, pois você não poderá visualizá-lo novamente).

### 2. Adicionar o PAT como Secret no Repositório
1. Vá para o seu repositório no GitHub.
2. Navegue até Settings>Secrets and variables>Actions.
3. Clique em New repository secret.
4. No campo Name, insira `PAT_TOKEN` (ou outro nome descritivo).
5. No campo Secret, cole o token gerado.
6. Clique em Add secret.
