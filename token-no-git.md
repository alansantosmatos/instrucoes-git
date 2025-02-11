Para criar um **Personal Access Token (PAT)** no GitHub, siga este passo a passo:

---

### 🔑 **1. Acessar as configurações do GitHub**
1. Vá para o GitHub: [https://github.com/settings/tokens](https://github.com/settings/tokens)
2. Clique em **"Generate new token"** (ou **"Tokens (classic)"**).

---

### 🔧 **2. Configurar o token**
1. **Dê um nome** ao token (ex: "Token para Git").
2. **Defina a expiração** (ou selecione "No expiration" se quiser que nunca expire).
3. **Escolha as permissões** (se for para Git, marque essas opções):
   - ✅ `repo` → Para acessar repositórios privados e públicos.
   - ✅ `workflow` → Se precisar rodar ações do GitHub Actions.
   - ✅ `write:packages` → Se for usar pacotes do GitHub.

4. Clique em **"Generate token"**.

---

### 📋 **3. Copiar e salvar o token**
- **IMPORTANTE**: Copie o token gerado **imediatamente**, pois ele não poderá ser visto novamente.
- Guarde-o em um local seguro.

---

### 🔗 **4. Usar o token no Git**
Se o Git pedir sua senha ao fazer `git push`, use o token no lugar da senha.

Caso precise atualizar as credenciais salvas:
```sh
git credential reject "https://github.com"
```

Se quiser salvar o token para não precisar digitar sempre:
```sh
git config --global credential.helper store
```
Depois, ao rodar um `git push`, o Git perguntará pelo token e salvará para usos futuros.

---

Agora você pode usar o token para autenticação no GitHub. Se precisar de mais alguma coisa, só perguntar! 🚀