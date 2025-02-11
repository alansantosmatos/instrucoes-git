Se você deseja **encerrar o uso do Git em um repositório local**, pode fazer o seguinte:

### 1️⃣ **Remover o repositório Git de um projeto**
Se quiser **desvincular completamente** o Git do seu projeto:
```sh
rm -rf .git
```
Isso **apaga** todas as configurações do Git, histórico de commits e a conexão com o repositório remoto.

---

### 2️⃣ **Desconectar o repositório remoto**
Se quiser apenas remover a conexão com o GitHub, sem apagar o histórico local:
```sh
git remote remove origin
```

---

### 3️⃣ **Sair do usuário Git configurado**
Se quiser remover suas credenciais do cache:
```sh
git credential reject "https://github.com"
```
Ou, para resetar todas as credenciais:
```sh
git credential reject https://
```

Se usou SSH:
```sh
ssh-add -D
```

---

### 4️⃣ **Desinstalar o Git (opcional)**
Se quiser remover o Git do sistema:

- **Linux (Ubuntu/Debian)**:
  ```sh
  sudo apt remove --purge git
  ```
- **Mac (Homebrew)**:
  ```sh
  brew uninstall git
  ```
- **Windows**:
  - Vá ao **Painel de Controle > Programas e Recursos** e desinstale o Git.

---

Se precisar reverter algo ou tiver dúvidas, me avise! 🚀