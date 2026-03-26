# ⚙️ Git Hooks

## 🧠 ¿Qué son?

Scripts que Git ejecuta automáticamente.

---

## 📌 Tipos

- pre-commit
- commit-msg
- pre-push

---

## 🧪 Ejemplo

Archivo:
.git/hooks/pre-commit

```bash
#!/bin/sh
echo "Corriendo checks..."
npm test