# Exercícios Práticos - Git e GitHub

## 📚 Guia de Exercícios para Aprender Git e GitHub

Este arquivo contém uma série de exercícios práticos para aprender os conceitos fundamentais do Git e GitHub, incluindo branches, commits, pull requests e gerenciamento de arquivos.

---

## 🎯 Objetivos de Aprendizado

Ao completar estes exercícios, você será capaz de:
- Criar e gerenciar repositórios Git
- Trabalhar com branches de forma eficiente
- Fazer commits significativos
- Colaborar usando pull requests
- Adicionar e gerenciar arquivos no repositório

---

## 📋 Pré-requisitos

- Git instalado no seu computador
- Conta no GitHub
- Editor de texto/código de sua preferência

---

## 🚀 Exercício 1: Configuração Inicial

### Tarefa 1.1: Configurar o Git
```bash
# Configure seu nome e email (substitua pelos seus dados)
git config --global user.name "Seu Nome"
git config --global user.email "seu.email@exemplo.com"

# Verifique a configuração
git config --list
```

### Tarefa 1.2: Clonar este repositório
```bash
# Clone o repositório para sua máquina local
git clone [URL_DO_REPOSITORIO]
cd harve-github-test
```

**✅ Checkpoint:** Você deve ter o repositório clonado localmente.

---

## 🌿 Exercício 2: Trabalhando com Branches

### Tarefa 2.1: Criar uma nova branch
```bash
# Crie uma branch com seu nome (ex: feature/joao-silva)
git checkout -b feature/[seu-nome]

# Verifique em qual branch você está
git branch
```

### Tarefa 2.2: Fazer alterações na sua branch
1. Crie um arquivo com seu nome: `[seu-nome].txt`
2. Adicione o seguinte conteúdo:
   ```
   Nome: [Seu Nome Completo]
   Data: [Data de hoje]
   Exercício: Aprendendo Git e GitHub

   Minhas linguagens de programação favoritas:
   1. [Linguagem 1]
   2. [Linguagem 2]
   3. [Linguagem 3]
   ```

### Tarefa 2.3: Commit das alterações
```bash
# Adicione o arquivo ao staging
git add [seu-nome].txt

# Faça o commit com uma mensagem descritiva
git commit -m "Adiciona arquivo pessoal de [seu-nome]"

# Verifique o histórico
git log --oneline
```

**✅ Checkpoint:** Você deve ter uma branch própria com um commit contendo seu arquivo pessoal.

---

## 📝 Exercício 3: Gerenciamento de Arquivos

### Tarefa 3.1: Adicionar múltiplos arquivos
1. Crie uma pasta chamada `projetos/[seu-nome]/`
2. Dentro dela, crie os seguintes arquivos:
   - `README.md` - Descrição de um projeto fictício
   - `codigo.py` - Um script Python simples
   - `notas.txt` - Suas anotações sobre Git

### Tarefa 3.2: Staging seletivo
```bash
# Adicione apenas o README.md
git add projetos/[seu-nome]/README.md

# Verifique o status
git status

# Adicione os demais arquivos
git add projetos/[seu-nome]/

# Faça o commit
git commit -m "Adiciona estrutura inicial do projeto [seu-nome]"
```

### Tarefa 3.3: Modificar e atualizar arquivos
1. Edite o arquivo `codigo.py` adicionando comentários
2. Modifique o `README.md` adicionando mais informações
3. Faça commits separados para cada alteração

```bash
# Commit das alterações no código
git add projetos/[seu-nome]/codigo.py
git commit -m "Adiciona comentários ao código Python"

# Commit das alterações no README
git add projetos/[seu-nome]/README.md
git commit -m "Atualiza documentação do projeto"
```

**✅ Checkpoint:** Você deve ter múltiplos commits organizados na sua branch.

---

## 🔄 Exercício 4: Pull Requests

### Tarefa 4.1: Enviar branch para o GitHub
```bash
# Envie sua branch para o repositório remoto
git push origin feature/[seu-nome]
```

### Tarefa 4.2: Criar Pull Request
1. Acesse o repositório no GitHub
2. Clique em "Compare & pull request"
3. Preencha o título: `Adiciona exercícios de [seu-nome]`
4. Na descrição, inclua:
   ```markdown
   ## Alterações realizadas
   - [ ] Criado arquivo pessoal
   - [ ] Adicionada estrutura de projeto
   - [ ] Implementados exercícios práticos

   ## Arquivos adicionados
   - [seu-nome].txt
   - projetos/[seu-nome]/README.md
   - projetos/[seu-nome]/codigo.py
   - projetos/[seu-nome]/notas.txt

   ## Observações
   [Adicione qualquer observação relevante]
   ```

### Tarefa 4.3: Review e merge
1. Peça para um colega revisar seu PR
2. Responda aos comentários (se houver)
3. Após aprovação, faça o merge

**✅ Checkpoint:** Seu pull request deve estar criado e pronto para review.

---

## 🔧 Exercício 5: Resolução de Conflitos

### Tarefa 5.1: Criar conflito intencional
1. Na branch `main`, edite o arquivo `exercicios-git-github.md`
2. Na sua branch, edite a mesma linha do mesmo arquivo
3. Tente fazer merge e resolva o conflito

```bash
# Volte para a main e faça uma alteração
git checkout main
git pull origin main

# Edite este arquivo (adicione seu nome na lista abaixo)
# Faça commit da alteração

# Volte para sua branch
git checkout feature/[seu-nome]

# Tente fazer merge da main
git merge main

# Se houver conflito, resolva editando o arquivo
# Depois faça commit da resolução
git add .
git commit -m "Resolve conflito de merge"
```

**✅ Checkpoint:** Você deve ter resolvido com sucesso um conflito de merge.

---

## 📊 Exercício 6: Histórico e Logs

### Tarefa 6.1: Explorar o histórico
```bash
# Veja o histórico completo
git log

# Veja o histórico resumido
git log --oneline

# Veja o histórico com gráfico
git log --graph --oneline --all

# Veja as alterações de um commit específico
git show [hash-do-commit]
```

### Tarefa 6.2: Comparar alterações
```bash
# Compare sua branch com a main
git diff main..feature/[seu-nome]

# Veja as diferenças não commitadas
git diff

# Veja as diferenças no staging
git diff --staged
```

**✅ Checkpoint:** Você deve conseguir navegar pelo histórico do projeto.

---

## 🎉 Exercício Final: Colaboração

### Tarefa Final: Contribuir para o projeto coletivo
1. Crie uma nova branch: `colaboracao/[seu-nome]`
2. Adicione seu nome à lista de colaboradores abaixo
3. Crie um arquivo `dicas/[seu-nome]-dicas.md` com suas dicas de Git
4. Faça um pull request bem documentado

### 👥 Lista de Colaboradores
<!-- Adicione seu nome aqui durante o exercício final -->
- Professor: [Nome do Professor]

### 💡 Dicas dos Alunos
<!-- Links para as dicas serão adicionados aqui -->

---

## 🏆 Critérios de Avaliação

### ✅ Lista de Verificação
- [ ] Configurou Git corretamente
- [ ] Criou branch própria
- [ ] Fez commits com mensagens descritivas
- [ ] Adicionou arquivos corretamente
- [ ] Criou pull request bem documentado
- [ ] Resolveu conflitos (se aplicável)
- [ ] Colaborou no exercício final

### 📈 Níveis de Proficiência

**Iniciante (⭐):**
- Completa exercícios 1-3
- Entende conceitos básicos de commit e branch

**Intermediário (⭐⭐):**
- Completa exercícios 1-5
- Consegue trabalhar com pull requests e resolver conflitos simples

**Avançado (⭐⭐⭐):**
- Completa todos os exercícios
- Demonstra boas práticas de colaboração e documentação

---

## 📚 Recursos Adicionais

### 🔗 Links Úteis
- [Documentação oficial do Git](https://git-scm.com/doc)
- [GitHub Guides](https://guides.github.com/)
- [Atlassian Git Tutorials](https://www.atlassian.com/git/tutorials)

### 🆘 Comandos de Emergência
```bash
# Desfazer último commit (mantém alterações)
git reset --soft HEAD~1

# Descartar alterações não commitadas
git checkout -- [arquivo]

# Voltar para estado anterior
git reset --hard HEAD

# Ver status atual
git status
```

---
