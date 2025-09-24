# Harve Git/GitHub – Repositório Didático

Repositório preparado para aulas e práticas guiadas de Git e GitHub. Aqui os alunos irão aprender fluxo de trabalho com branches, commits, pull requests, resolução de conflitos e colaboração.

## Conteúdo Principal
- `exercicios-git-github.md`: trilha de exercícios passo a passo (configuração, branches, commits, PRs, conflitos, histórico).
- `estrutura-exercicios.md`: estrutura de pastas recomendada, exemplos de conteúdo e checklist para professores.
- `.pre-commit-config.yaml`: configuração de hooks para garantir qualidade mínima nos commits.

## Pré-requisitos
- Git instalado
- Conta no GitHub
- Editor de código (VS Code recomendado)

## Como começar
1. Faça o fork (se aplicável) e clone o repositório:
   ```bash
   git clone <URL_DO_REPOSITORIO>
   cd harve-github-test
   ```
2. Configure seu Git (se ainda não fez):
   ```bash
   git config --global user.name "Seu Nome"
   git config --global user.email "seu.email@exemplo.com"
   ```
3. Leia e siga `exercicios-git-github.md`.

## Fluxo de trabalho recomendado
1. Crie uma branch a partir da `main`:
   ```bash
   git checkout -b feature/seu-nome
   ```
2. Faça alterações pequenas e com commits descritivos:
   ```bash
   git add <arquivos>
   git commit -m "Adiciona <descrição curta>"
   ```
3. Publique e abra um Pull Request:
   ```bash
   git push origin feature/seu-nome
   ```
4. Solicite revisão, responda comentários e faça o merge após aprovação.

## Convenções
- Prefixos de branch: `feature/`, `bugfix/`, `hotfix/`, `chore/`.
- Mensagens de commit no imperativo: "Adiciona", "Atualiza", "Corrige".
- Evite commits grandes; prefira mudanças pequenas e focadas.

## Estrutura sugerida (resumo)
Veja detalhes em `estrutura-exercicios.md`. Exemplo:
```
projetos/
  └── seu-nome/
      ├── README.md
      ├── codigo.py
      └── notas.txt
```

## Dicas rápidas
- Ver diferenças antes do commit: `git diff --staged`
- Histórico resumido: `git log --oneline --graph --all`
- Corrigir trailing spaces: rode o pre-commit ou ajuste no editor

## Suporte e dúvidas
Abra uma Issue no GitHub com título claro e passos para reproduzir, quando aplicável.
