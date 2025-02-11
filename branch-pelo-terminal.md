Para criar uma nova branch no GitHub pelo terminal, siga estes passos:

---

### 1️⃣ **Criar uma nova branch localmente**
```sh
git branch nome-da-branch
```
ou crie e já troque para ela:
```sh
git switch -c nome-da-branch
```
(método antigo: `git checkout -b nome-da-branch`)

---

### 2️⃣ **Enviar a nova branch para o GitHub**
```sh
git push -u origin nome-da-branch
```

Isso cria a branch no repositório remoto do GitHub e define o rastreamento da branch local com a remota.

---

### 3️⃣ **Confirmar que a branch foi criada no GitHub**
Após o push, vá até o repositório no GitHub e veja se a nova branch aparece na lista de branches.

---

### 🔄 **Se quiser trocar de branch no futuro:**
```sh
git switch nome-da-branch
```
ou (método antigo):
```sh
git checkout nome-da-branch
```

Agora pode trabalhar na nova branch e fazer commits normalmente.

Se precisar de mais alguma coisa, só perguntar! 🚀