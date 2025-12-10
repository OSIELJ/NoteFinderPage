# 🚀 Guia: Como publicar no GitHub Pages

## Passo a passo completo

### 1. Criar um repositório no GitHub

1. Acesse [github.com](https://github.com) e faça login
2. Clique no botão **"+"** no canto superior direito
3. Selecione **"New repository"**
4. Preencha:
   - **Repository name**: `NoteFinderPage` (ou outro nome de sua preferência)
   - **Description**: "Página web do aplicativo NoteFinder"
   - Marque como **Public** (GitHub Pages gratuito só funciona com repositórios públicos)
   - **NÃO** marque "Initialize this repository with a README"
5. Clique em **"Create repository"**

### 2. Inicializar Git no seu projeto (se ainda não tiver)

Abra o terminal/PowerShell na pasta do projeto e execute:

```bash
git init
```

### 3. Adicionar todos os arquivos

```bash
git add .
```

### 4. Fazer o primeiro commit

```bash
git commit -m "Primeira versão da página NoteFinder"
```

### 5. Conectar ao repositório do GitHub

Substitua `SEU_USUARIO` pelo seu nome de usuário do GitHub:

```bash
git remote add origin https://github.com/SEU_USUARIO/NoteFinderPage.git
```

### 6. Enviar os arquivos para o GitHub

```bash
git branch -M main
git push -u origin main
```

Você precisará fazer login no GitHub quando solicitado.

### 7. Ativar o GitHub Pages

1. No GitHub, vá até o seu repositório
2. Clique em **"Settings"** (Configurações)
3. No menu lateral, clique em **"Pages"**
4. Em **"Source"**, selecione:
   - Branch: **main**
   - Folder: **/ (root)**
5. Clique em **"Save"**

### 8. Acessar sua página

Após alguns minutos, sua página estará disponível em:
```
https://SEU_USUARIO.github.io/NoteFinderPage/
```

## ⚠️ Importante

- O GitHub Pages pode levar alguns minutos para publicar pela primeira vez
- Qualquer atualização que você fizer, precisará fazer commit e push novamente
- A URL será sempre: `https://SEU_USUARIO.github.io/NOME_DO_REPOSITORIO/`

## 📝 Comandos úteis para futuras atualizações

Quando fizer alterações nos arquivos:

```bash
git add .
git commit -m "Descrição das mudanças"
git push
```

## 🔧 Solução de problemas

**Página não aparece?**
- Aguarde 5-10 minutos após ativar o GitHub Pages
- Verifique se o repositório é público
- Confirme que o arquivo `index.html` está na raiz do repositório
- Verifique se a branch está configurada corretamente nas Settings

**Erro 404?**
- Certifique-se de que o arquivo se chama exatamente `index.html` (com 'i' minúsculo)
- Verifique se todos os arquivos foram enviados (styles.css, script.js)

---

**Dica**: Você pode usar um domínio personalizado depois nas configurações do GitHub Pages!

