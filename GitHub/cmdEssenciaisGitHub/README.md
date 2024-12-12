<div align="center">

<!-- Imagem com efeito de neumorfismo e gradiente das cores da bandeira do Brasil -->
<img src="https://github.githubassets.com/images/modules/logos_page/GitHub-Mark.png" 
     width="10%" 
     style="border-radius: 50%; 
            background: linear-gradient(135deg, #009739, #FFCC29, #005AA7); /* Gradiente da bandeira do Brasil */
            box-shadow: 10px 10px 20px rgba(0, 0, 0, 0.1), -10px -10px 20px rgba(255, 255, 255, 0.7); /* Efeito neumorfismo */
            padding: 15px; /* Distância entre a imagem e a borda */
            border: 5px solid #fff; /* Borda suave */
            margin-top: 20px;" />

[![Licença MIT](https://img.shields.io/badge/license-MIT-blue.svg)](LICENSE)
[![GitHub Stars](https://img.shields.io/github/stars/seu-usuario/seu-repositorio?style=social)](https://github.com/seu-usuario/seu-repositorio/stargazers)

</div>

## 📋 Índice

- [Introdução](#-introdução)
- [Configuração Inicial](#-configuração-inicial)
- [Comandos Básicos](#-comandos-básicos)
- [Branches](#-branches)
- [Colaboração](#-colaboração)
- [Sincronização](#-sincronização)
- [Desfazendo Alterações](#-desfazendo-alterações)
- [Dicas Úteis](#-dicas-úteis)

## 🎯 Introdução

Este guia fornece uma visão geral dos comandos mais importantes do Git e GitHub, essenciais para o desenvolvimento de software moderno e colaboração em equipe.

## ⚙️ Configuração Inicial

```bash
# Configurar nome de usuário
git config --global user.name "Seu Nome"

# Configurar email
git config --global user.email "seu-email@exemplo.com"

# Verificar configurações
git config --list
```

## 🔰 Comandos Básicos

### Iniciando um Repositório

```bash
# Inicializar um novo repositório
git init

# Clonar um repositório existente
git clone <url-do-repositorio>
```

### Gerenciando Alterações

```bash
# Verificar status do repositório
git status

# Adicionar arquivos ao staging
git add <arquivo>
git add .  # adiciona todos os arquivos

# Criar um commit
git commit -m "mensagem do commit"

# Visualizar histórico de commits
git log
```

## 🌿 Branches

```bash
# Criar uma nova branch
git branch <nome-da-branch>

# Mudar para uma branch
git checkout <nome-da-branch>

# Criar e mudar para uma nova branch
git checkout -b <nome-da-branch>

# Listar branches
git branch

# Deletar uma branch
git branch -d <nome-da-branch>
```

## 👥 Colaboração

```bash
# Adicionar um repositório remoto
git remote add origin <url-do-repositorio>

# Enviar alterações para o repositório remoto
git push origin <nome-da-branch>

# Baixar alterações do repositório remoto
git pull origin <nome-da-branch>
```

## 🔄 Sincronização

```bash
# Atualizar repositório local com alterações remotas
git fetch

# Mesclar branches
git merge <nome-da-branch>

# Baixar e mesclar alterações
git pull
```

## ↩️ Desfazendo Alterações

```bash
# Desfazer alterações em arquivos não staged
git checkout -- <arquivo>

# Desfazer alterações staged
git reset HEAD <arquivo>

# Desfazer último commit mantendo as alterações
git reset --soft HEAD~1

# Desfazer último commit removendo as alterações
git reset --hard HEAD~1
```

## 💡 Dicas Úteis

### Aliases Úteis

```bash
# Configurar aliases para comandos comuns
git config --global alias.st status
git config --global alias.co checkout
git config --global alias.br branch
git config --global alias.ci commit
```

### Ignorando Arquivos

Crie um arquivo `.gitignore` na raiz do projeto e adicione os padrões de arquivos que devem ser ignorados:

```plaintext
node_modules/
.env
*.log
.DS_Store
```

## 🔑 Boas Práticas

1. **Commits Significativos**
   - Escreva mensagens claras e descritivas
   - Use verbos no imperativo
   - Mantenha commits pequenos e focados

2. **Branches**
   - Use branches para novas features
   - Mantenha a main/master sempre estável
   - Delete branches após o merge

3. **Pull Requests**
   - Faça code review
   - Teste antes de mergear
   - Mantenha a discussão focada

## 📚 Recursos Adicionais

- [Documentação Oficial do Git](https://git-scm.com/doc)
- [GitHub Guides](https://guides.github.com/)
- [Git Cheat Sheet](https://education.github.com/git-cheat-sheet-education.pdf)

## 📄 Licença

Este projeto está sob a licença MIT. Veja o arquivo [LICENSE](LICENSE) para mais detalhes.

---

<div align="center">

⭐ Se este guia foi útil, considere dar uma estrela no repositório!

</div>
