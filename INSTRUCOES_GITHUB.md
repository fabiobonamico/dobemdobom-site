# 📝 Instruções para Criar Repositório no GitHub

## Passo 1: Verificar/Criar Repositório Git Local

Se o Git ainda não estiver inicializado, execute:

```powershell
git init
```

## Passo 2: Verificar Arquivos para Commit

```powershell
git status
```

## Passo 3: Adicionar Arquivos ao Stage

```powershell
git add .
```

## Passo 4: Fazer Commit Inicial

```powershell
git commit -m "Initial commit: Projeto Tatu do Bem - ArtisTree"
```

## Passo 5: Criar Repositório no GitHub

### Opção A: Via GitHub CLI (gh)

Se você tem o GitHub CLI instalado:

```powershell
gh repo create dobemdobom-site --public --source=. --remote=origin --push
```

### Opção B: Via Site do GitHub (Recomendado)

1. Acesse: https://github.com/new
2. Nome do repositório: `dobemdobom-site` (ou outro nome de sua escolha)
3. Escolha: **Public** ou **Private**
4. **NÃO** marque "Initialize this repository with a README"
5. Clique em **"Create repository"**

## Passo 6: Conectar Repositório Local ao GitHub

Após criar o repositório no GitHub, você receberá uma URL. Execute:

```powershell
git remote add origin https://github.com/SEU_USUARIO/dobemdobom-site.git
```

Substitua `SEU_USUARIO` pelo seu nome de usuário do GitHub.

## Passo 7: Fazer Push do Código

```powershell
git branch -M main
git push -u origin main
```

## ✅ Verificação Final

Após o push, verifique:

1. Acesse: https://github.com/SEU_USUARIO/dobemdobom-site
2. Verifique se todos os arquivos foram enviados
3. Confirme que o README.md aparece corretamente

---

## 🔐 Autenticação

Se você receber erro de autenticação:

### Opção 1: Personal Access Token
1. Vá em: GitHub → Settings → Developer settings → Personal access tokens → Tokens (classic)
2. Crie um novo token com permissões de `repo`
3. Use o token como senha quando solicitado

### Opção 2: GitHub CLI (mais fácil)
```powershell
gh auth login
```

---

## 📋 Checklist Final

- [ ] Git inicializado
- [ ] Arquivos commitados
- [ ] Repositório criado no GitHub
- [ ] Remote origin configurado
- [ ] Push realizado com sucesso
- [ ] Arquivos visíveis no GitHub

