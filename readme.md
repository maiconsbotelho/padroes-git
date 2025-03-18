# 📌 Comandos GIT, Padrões de Branches e Commits

## 💻 **Principais Comandos Git**

### 🔧 **Comandos Básicos**

- `git init` → Inicializa um repositório Git no diretório atual.
- `git clone <url-do-repositorio>` → Clona um repositório remoto para o seu diretório local.
- `git status` → Exibe o status atual do repositório (arquivos modificados, não rastreados, etc.).
- `git add <arquivo>` → Adiciona um arquivo específico ao índice de preparação.
- `git add .` → Adiciona todos os arquivos modificados ao índice de preparação.
- `git commit -m "mensagem"` → Realiza um commit com a mensagem fornecida.
- `git push` → Envia as alterações locais para o repositório remoto.
- `git pull` → Atualiza o repositório local com as alterações do repositório remoto.
- `git fetch` → Baixa as últimas alterações do repositório remoto sem aplicá-las.
- `git merge <branch>` → Mescla as alterações de uma branch em outra.
- `git branch` → Lista todas as branches locais.
- `git branch <nome-da-branch>` → Cria uma nova branch.
- `git checkout <branch>` → Altera para a branch especificada.
- `git checkout -b <nome-da-branch>` → Cria uma nova branch e alterna para ela.
- `git log` → Exibe o histórico de commits.

### 🔄 **Comandos para Gerenciamento de Branches**

- `git merge <branch>` → Mescla uma branch em outra.
- `git rebase <branch>` → Aplica as alterações de uma branch sobre outra.
- `git branch -d <branch>` → Exclui uma branch local.
- `git branch -D <branch>` → Força a exclusão de uma branch local, mesmo se não estiver totalmente mesclada.
- `git reset --hard` → Desfaz todas as alterações locais e redefine o repositório para o último commit.
- `git reset <commit>` → Reseta o repositório para o estado de um commit específico.

### 🔀 **Comandos para Resolução de Conflitos**

- `git mergetool` → Abre uma ferramenta de merge para resolver conflitos.
- `git diff` → Exibe as diferenças entre o repositório local e o remoto, ou entre commits.

### 🧹 **Comandos de Limpeza e Manutenção**

- `git clean -fd` → Remove arquivos não rastreados no diretório de trabalho.
- `git gc` → Realiza uma coleta de lixo, otimizando o repositório.

### 🌐 **Comandos para Repositórios Remotos**

- `git remote add <nome> <url-do-repositorio>` → Adiciona um repositório remoto.
- `git remote -v` → Exibe os repositórios remotos configurados.
- `git push <remote> <branch>` → Envia a branch local para o repositório remoto.
- `git pull <remote> <branch>` → Baixa as últimas alterações de uma branch no repositório remoto.

---

## 🌿 **Padrões de Nomes de Branches**

### 🌍 **Principais Branches Globais**

- `Initial commit` → Commit inicial
- `main` → Produção
- `develop` → Desenvolvimento principal
- `staging` → Ambiente de homologação/testes
- `preprod` → Pré-produção
- `qa` → Qualidade/Testes

### 🚀 **Branches para Funcionalidades e Melhorias**

- `feature/nome-da-feature` → Nova funcionalidade
- `enhancement/nome-da-melhoria` → Melhorias em funcionalidades existentes
- `improvement/nome-da-melhoria` → Melhorias gerais

### 🔧 **Branches para Correções de Erros**

- `fix/nome-do-fix` → Correção de bug
- `bugfix/nome-do-bugfix` → Correção de bug (alternativo)
- `hotfix/nome-do-hotfix` → Correção urgente em produção
- `patch/nome-do-patch` → Pequenas correções ou ajustes rápidos

### 📌 **Branches para Tarefas e Manutenção**

- `task/nome-da-task` → Alterações menores ou ajustes técnicos
- `chore/nome-da-tarefa` → Manutenção e configuração
- `maintenance/nome-da-manutencao` → Atualizações não relacionadas a código

### 📖 **Branches para Documentação**

- `docs/nome-da-doc` → Atualizações na documentação
- `documentation/nome-da-doc` → Alternativo para documentação

### 📦 **Branches para Builds, Releases e Versões**

- `release/x.y.z` → Preparação de uma nova versão
- `build/nome-do-build` → Build específico
- `version/nome-da-versao` → Controle de versões

### 🔄 **Branches para Refatoração e Otimização**

- `refactor/nome-da-refatoracao` → Refatoração de código
- `restructure/nome-da-reestruturacao` → Reestruturação geral
- `cleanup/nome-da-limpeza` → Remoção de código desnecessário

### 🧪 **Branches para Testes e Experimentos**

- `test/nome-do-teste` → Testes diversos
- `experiment/nome-do-experimento` → Teste de novas abordagens
- `sandbox/nome-da-sandbox` → Código experimental

### 📌 **Branches para Segurança**

- `security/nome-da-correção` → Correções relacionadas à segurança
- `dependabot/npm_and_yarn/dependency-name` → Atualização automática de dependências (GitHub Dependabot)

### 🎟️ **Branches Baseadas em Ticket/JIRA**

- `feature/PROJ-123-nome-da-feature`
- `fix/PROJ-456-corrigir-bug`
- `hotfix/PROJ-789-erro-em-producao`
- `task/PROJ-101-ajustar-layout`

---

## 🔥 **Padrões de Mensagens de Commit (Conventional Commits)**

### 🚀 **Commits para o Primeiro Commit**

- `Initial commit` → Padrão mais utilizado para iniciar o repositório.
- `chore: initial commit` → Indica um commit inicial seguindo o Conventional Commits.
- `build: iniciar configuração do projeto` → Utilizado para configurar dependências e builds iniciais.
- `feat: iniciar estrutura do projeto` → Define a base do código.
- `docs: adicionar README inicial` → Indica um commit inicial contendo apenas documentação.

### 🚀 **Commits para Funcionalidades e Melhorias**

- `feat` → Indica a inclusão de um novo recurso. Relaciona-se com o **MINOR** no versionamento semântico.
- `enhancement` → Utilizado para melhorias incrementais em funcionalidades já existentes.

### 🔧 **Commits para Correções**

- `fix` → Utilizado para corrigir um **bug** no código. Relaciona-se com o **PATCH** no versionamento semântico.
- `hotfix` → Indica uma correção urgente aplicada diretamente em produção.

### 📖 **Commits para Documentação**

- `docs` → Indica mudanças na **documentação** do projeto, como README, comentários e guias. **Não inclui alterações no código-fonte.**

### 🧪 **Commits para Testes**

- `test` → Indica criação, alteração ou remoção de testes unitários. **Não inclui mudanças no código-fonte.**

### 🛠️ **Commits para Infraestrutura e Dependências**

- `build` → Utilizado para modificações em arquivos de **build e dependências**.
- `ci` → Indica alterações relacionadas à **integração contínua (CI/CD)**.

### 🎨 **Commits para Estilização e Formatação**

- `style` → Indica mudanças de formatação, como indentação, remoção de espaços extras, linting, **sem alterar a lógica do código**.

### 🔄 **Commits para Refatoração e Otimização**

- `refactor` → Indica mudanças internas que **não alteram a funcionalidade** do código, como reestruturação lógica.
- `perf` → Utilizado para **melhorias de performance** sem alterar a funcionalidade.
- `restructure` → Indica mudanças na arquitetura do projeto.
- `cleanup` → Utilizado para remover código comentado, trechos desnecessários ou refatorações para legibilidade.

### 🛠️ **Commits para Manutenção**

- `chore` → Indica **tarefas de manutenção**, como configuração de pacotes, atualizações de dependências e ajustes de ambiente.
- `raw` → Utilizado para mudanças em arquivos de configuração, parâmetros e datasets.

### 🗑️ **Commits para Remoção**

- `remove` → Indica a **exclusão de arquivos, diretórios ou funcionalidades obsoletas**.

### 🎟️ **Commits Baseados em Ticket/JIRA**

- `feat(PROJ-123): adicionar filtro por data` → Exemplo de feature ligada a um ticket.
- `fix(PROJ-456): corrigir erro ao salvar usuário` → Exemplo de correção de bug vinculado a um ticket.
- `task(PROJ-789): ajustar layout da página inicial` → Exemplo de tarefa vinculada a um ticket.

---
