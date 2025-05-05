
# 📘 Git Básico para Desenvolvedores (Resumo Didático)

Este guia vai te ajudar a entender e usar os principais comandos do Git no dia a dia do desenvolvimento.

---

## ✅ Fluxo de Trabalho Comum

1. **Atualize seu repositório com as últimas mudanças do GitHub**:
```bash
git pull origin main
```

2. **Verifique o que foi modificado**:
```bash
git status
```

3. **Adicione as alterações (todos os arquivos)**:
```bash
git add .
```

4. **Crie um commit com uma mensagem clara**:
```bash
git commit -m "Mensagem explicando a mudança"
```

5. **Envie as alterações para o GitHub**:
```bash
git push origin main
```

---

## 🔍 Visualizar histórico de versões

```bash
git log
```
Mostra todos os commits feitos no projeto.

---

## 🔙 Voltar para uma versão anterior

### Ver o ID do commit:

```bash
git log
```
Copie os primeiros caracteres do commit que você quer voltar. Ex: `a1b2c3d4`

### Voltar temporariamente (modo leitura):

```bash
git checkout a1b2c3d4
```

### Voltar permanentemente (apaga o que veio depois):

```bash
git reset --hard a1b2c3d4
```

### Voltar e manter arquivos como estão (sem apagar):

```bash
git reset --soft a1b2c3d4
```

---

## 🗑️ Desfazer o último commit (permanente!):

```bash
git reset --hard HEAD~1
```

---

## 🏷️ Marcar uma versão importante (tag):

```bash
git tag -a v1.0 -m "Versão estável 1.0"
git push origin v1.0
```

### Voltar para a tag:
```bash
git checkout v1.0
```

---

## 💡 Dica: Commits pequenos e frequentes
Crie um commit para cada parte da tarefa. Exemplo:
- "Cria estrutura HTML da página inicial"
- "Adiciona estilos para layout responsivo"
- "Corrige erro no botão de envio"

---

## 🎯 Conclusão

Com esses comandos, você consegue versionar seu projeto com segurança, trabalhar em equipe e nunca mais perder código por erro.

