# 🌟 Guia de Boas Práticas - Git & GitHub

Este guia reúne recomendações para manter seu fluxo de trabalho organizado e profissional, utilizando os comandos aprendidos no curso.

---

### 1. 📝 Mensagens de Commit Semânticas
Evite mensagens vagas. Uma boa mensagem de commit deve explicar **o que** foi feito.
* **Evite:** `git commit -m "alterações"`.
* **Prefira:** `git commit -m "feat: adiciona explicações sobre git stash"`.

### 2. 🧱 Commits Atômicos
Tente realizar commits pequenos que foquem em apenas uma tarefa. Isso facilita o uso do `git restore` ou `git reset` caso algo dê errado, pois você não perde grandes blocos de trabalho de uma só vez.

### 3. 🛡️ Segurança e Limpeza com .gitignore
Mantenha seu repositório limpo. Use o arquivo `.gitignore` para impedir que arquivos temporários ou pastas de configuração sejam rastreados.
* Exemplo: `echo node_modules/ >> .gitignore`.

### 4. 🌿 Fluxo de Trabalho com Branches
Para manter a integridade da sua branch principal (`main`), sempre crie ramificações para novas funcionalidades ou testes.
* Use `git checkout -b nome-da-branch` para isolar seu trabalho.
* Realize o `git merge` apenas quando o código estiver testado e estável.

### 5. 🔄 Sincronização Constante
Trabalhar com repositórios remotos exige atenção ao estado do código no servidor.
* **Antes de iniciar:** Use `git pull` para baixar e mesclar as alterações mais recentes.
* **Ao finalizar:** Use `git push` para enviar seu progresso para o GitHub.

### 6. 🔍 Revisão antes do Commit
Sempre verifique o que será enviado para a área de preparação.
* Utilize o `git status` com frequência para ver o estado dos seus arquivos.
* Use o `git diff` para revisar as alterações nas linhas de código antes de confirmar.

---
_Dica: Adotar essas práticas ajuda muito na colaboração com outros desenvolvedores!_