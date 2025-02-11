Esse erro indica que você não tem permissão para enviar código para o repositório `alura-cursos/3997-calculadora.git`. Aqui estão algumas soluções para resolver o problema:

---

### 🔍 **1. Verifique se está autenticado corretamente**
Se estiver usando HTTPS, tente reautenticar com seu usuário:

```sh
git remote set-url origin https://github.com/seu-usuario/seu-repo.git
git push origin main
```

Caso precise de um **Personal Access Token (PAT)** (em vez de senha), gere um [token no GitHub](https://github.com/settings/tokens) e use ele no lugar da senha.

---

### 🔑 **2. Se estiver usando SSH, verifique sua chave SSH**
Se clonou o repositório via SSH (`git@github.com:...`), verifique se sua chave SSH está configurada corretamente:

1. Liste suas chaves públicas:
   ```sh
   cat ~/.ssh/id_rsa.pub
   ```
   ou  
   ```sh
   cat ~/.ssh/id_ed25519.pub
   ```

2. Adicione a chave ao GitHub:
   - Vá para **Settings > SSH and GPG keys** no GitHub.
   - Clique em **New SSH Key**, cole a chave pública e salve.

3. Teste a conexão:
   ```sh
   ssh -T git@github.com
   ```
   Se tudo estiver certo, deve aparecer uma mensagem como:
   ```
   Hi seu-usuario! You've successfully authenticated, but GitHub does not provide shell access.
   ```

---

### 🔄 **3. Verifique se tem permissão no repositório**
Se o repositório `alura-cursos/3997-calculadora.git` não for seu, peça ao dono que te adicione como colaborador:

- O dono do repositório deve ir até **Settings > Collaborators** e te adicionar.

---

### 🛠 **4. Se precisar clonar um fork**
Se o repositório pertence a outra pessoa e você quer fazer alterações, você pode **fazer um fork** e trabalhar no seu próprio repositório:

1. Vá até o repositório no GitHub e clique em **Fork**.
2. Clone seu fork:
   ```sh
   git clone https://github.com/seu-usuario/3997-calculadora.git
   ```
3. Faça alterações e envie para o seu repositório:
   ```sh
   git push origin main
   ```

Depois, crie um **Pull Request (PR)** para o repositório original.

---

Se o problema continuar, me avise! 🚀