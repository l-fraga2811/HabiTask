# Contribute to Habitask!

Eae galera, beleza? Seguinte então, vamos continuar como falamos no grupo, separando entre as pastas Backend e Frontend.
Os prs serão aceitos conforme a disponibilidade dos tech leaders, caso precisem de ajuda podem chamar alguém que é mais experiente mas **não desistam!** Esse projeto é um passo gigante na carreira de vocês.


---

### **1. Fluxo Básico de Trabalho**

Sempre sigam estas etapas:

1. **Atualizem a branch `develop` antes de começar:**
    
    ```bash
    git checkout develop
    git pull origin develop
    
    ```
    
2. **Criem uma branch para sua tarefa:**
    - Nomes claros e organizados:
        - `feature/nome-da-funcionalidade` (novas funcionalidades).
        - `bugfix/descricao-do-bug` (para corrigir problemas).
        Exemplo:
    
    ```bash
    git checkout -b feature/login-page
    
    ```
    
3. **Trabalhem apenas na sua branch:**
Façam as mudanças necessárias e salvem:
    
    ```bash
    git add .
    git commit -m "Descrição clara do que foi feito"
    
    ```
    
4. **Mantenham a branch atualizada:**
Durante o trabalho, sincronizem a branch com `develop` para evitar conflitos:
    
    ```bash
    git checkout develop
    git pull origin develop
    git checkout feature/login-page
    git merge develop
    
    ```
    
5. **Finalizem e enviem a branch para o repositório:**
    
    ```bash
    git push origin feature/login-page
    
    ```
    
6. **Abram um Pull Request (PR):**
    - Acessem o repositório no GitHub.
    - Criem um PR da branch para a branch `develop`.
    - **Eu revisarei o PR e farei o merge após aprovação.**

---

### **2. Regras para Trabalhar em Equipe**

1. **Nunca trabalhem diretamente na branch `develop`.**
    
    Sempre criem uma branch para cada tarefa.
    
2. **Comuniquem alterações importantes.**
    
    Se vocês mexerem em algo que pode afetar os outros, avisem no grupo.
    
3. **PRs pequenos e rápidos.**
    
    Dividam o trabalho em partes menores para facilitar a revisão.
    
4. **Sem merges automáticos.**
    
    Só o (PM) pode aprovar os PRs e realizar o merge na branch `develop`.
    
5. **Resolvam conflitos antes de enviar o PR.**
    
    Caso surjam conflitos, resolvam na sua branch antes de abrir o PR.
    

---

### **3. O que Fazer se Houver Conflito**

Conflitos acontecem quando duas pessoas alteram o mesmo arquivo. Para resolver:

1. Atualizem sua branch com `develop`:
    
    ```bash
    git checkout develop
    git pull origin develop
    git checkout feature/sua-branch
    git merge develop
    
    ```
    
2. Usem um editor (como VS Code ou GitHub Desktop) para resolver os conflitos.
3. Depois de corrigir, salvem as mudanças:
    
    ```bash
    git add .
    git commit -m "Conflitos resolvidos"
    git push origin feature/sua-branch
    
    ```
    
4. Depois disso, abram o PR para revisão.

---

### **4. Resumo Visual do Fluxo**

1. Atualizem `develop`.
2. Criem uma branch para a tarefa.
3. Trabalhem na branch.
4. Atualizem a branch com `develop`.
5. Enviem o PR para revisão.

---
```bash
EventManager/
│── frontend/
│   ├── public/
│   ├── src/
│   │   ├── components/
│   │   ├── pages/
│   │   ├── styles/
│   │   ├── hooks/
│   │   ├── services/
│   │   ├── contexts/
│   ├── .env
│   ├── vite.config.ts
│   ├── next.config.js
│   ├── package.json
│   ├── dockerfile
│
│── backend/
│   ├── src/
│   │   ├── main/java/com/eventmanager/
│   │   │   ├── controllers/
│   │   │   ├── models/
│   │   │   ├── repositories/
│   │   │   ├── services/
│   │   │   ├── dtos/
│   │   │   ├── config/
│   │   │   ├── EventManagerApplication.java
│   ├── .env
│   ├── pom.xml
│   ├── application.yml
│   ├── dockerfile
│
│── database/
│   ├── docker-compose.yml
│   ├── init.sql
│
│── docs/
│   ├── [README.md](http://readme.md/)
│   ├── [API.md](http://api.md/)
│
│── .gitignore
│── [README.md](http://readme.md/)
│── docker-compose.yml
```
