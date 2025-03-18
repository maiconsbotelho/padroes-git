# 📌 Padrões de Nomes de Branches e Commits

## 🌿 **Padrões de Nomes de Branches**

### 🌍 **Principais Branches Globais**

- `main` → Produção
- `develop` → Desenvolvimento principal
- `staging` → Ambiente de homologação/testes
- `preprod` → Pré-produção
- `qa` → Qualidade/Testes

### 🚀 **Branches para Funcionalidades e Melhorias**

- `feature/nome-da-feature` → Nova funcionalidade
- `feat/nome-da-feature` → Nova funcionalidade (alternativo)
- `enhancement/nome-da-melhoria` → Melhorias em funcionalidades existentes
- `improvement/nome-da-melhoria` → Melhorias gerais

### 🔧 **Branches para Correções de Erros**

- `fix/nome-do-fix` → Correção de bug
- `bugfix/nome-do-bugfix` → Correção de bug (alternativo)
- `hotfix/nome-do-hotfix` → Correção urgente em produção
- `patch/nome-do-patch` → Pequenas correções ou ajustes rápidos

### 📌 **Branches para Tarefas e Manutenção**

- `task/nome-da-task` → Tarefa técnica ou administrativa
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

### 🚀 **Commits para Funcionalidades e Melhorias**

- `feat: adicionar nova funcionalidade`
- `feat: implementar login social`
- `enhancement: melhorar carregamento da página`
- `improvement: otimizar algoritmo de busca`

### 🔧 **Commits para Correções**

- `fix: corrigir erro ao carregar usuários`
- `bugfix: corrigir erro na API de autenticação`
- `hotfix: corrigir erro crítico em produção`

### 📌 **Commits para Manutenção e Refatoração**

- `refactor: reorganizar lógica de validação`
- `restructure: alterar arquitetura do projeto`
- `cleanup: remover código não utilizado`

### 🛠️ **Commits para Infraestrutura e Dependências**

- `chore: atualizar dependências`
- `build: atualizar versão do Node.js`
- `ci: corrigir workflow do GitHub Actions`

### 📖 **Commits para Documentação**

- `docs: atualizar README com novas instruções`
- `docs: adicionar diagrama de arquitetura`

### 🧪 **Commits para Testes**

- `test: adicionar testes unitários`
- `test: corrigir falha nos testes de integração`

### 🔒 **Commits para Segurança**

- `security: corrigir vulnerabilidade XSS`

### 🎨 **Commits para Estilização e Formatação**

- `style: corrigir indentação e remover espaços extras`
- `style: aplicar novo padrão de cores`

### 🛠️ **Commits para Performance**

- `perf: otimizar consulta ao banco de dados`

### 🎟️ **Commits Baseados em Ticket/JIRA**

- `feat(PROJ-123): adicionar filtro por data`
- `fix(PROJ-456): corrigir erro ao salvar usuário`
- `task(PROJ-789): ajustar layout da página inicial`
