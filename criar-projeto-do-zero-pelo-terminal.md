Para criar um projeto do zero e enviá-lo para o GitHub pelo terminal, siga este passo a passo:

---

### 📌 **1. Criar o projeto e inicializar o Git**
```sh
mkdir meu-projeto
cd meu-projeto
git init  # Inicializa o repositório Git
```

---

### 📝 **2. Criar um arquivo no projeto** (opcional)
Se quiser, adicione um arquivo para testar:

```sh
echo "# Meu Projeto" > README.md
```

---

### 📂 **3. Adicionar os arquivos ao Git**
```sh
git add .
```

---

### 💾 **4. Criar um commit**
```sh
git commit -m "Primeiro commit"
```

---

### 🔗 **5. Criar um repositório no GitHub**
- Acesse [GitHub](https://github.com/) e crie um novo repositório (sem inicializar com `README.md` ou `.gitignore`).
- Copie a URL do repositório, por exemplo:  
  `https://github.com/seu-usuario/meu-projeto.git`

---

### 🚀 **6. Conectar o repositório local ao GitHub**
```sh
git remote add origin https://github.com/seu-usuario/meu-projeto.git
```

---

### 📤 **7. Enviar os arquivos para o GitHub**
```sh
git push -u origin main
```
Se a branch principal for `master`, use:
```sh
git push -u origin master
```

---

### 🎉 **8. Verificar no GitHub**
Acesse o repositório no GitHub e veja se os arquivos foram enviados.

Agora, sempre que quiser atualizar o projeto:
```sh
git add .
git commit -m "Descrição das mudanças"
git push origin main
```

Se precisar de mais alguma coisa, só avisar! 🚀