# ⚙️ Git Hooks - Explicación Completa

Los hooks son scripts que Git ejecuta automáticamente en ciertos eventos.

---

## 📌 ¿Qué son?

Son scripts ubicados en:

```
.git/hooks/
```

---

## 🔧 Tipos principales

### pre-commit

Se ejecuta antes de hacer commit.

```bash
.git/hooks/pre-commit
```

**¿Qué hace?**
- Permite validar código antes de commit

**Ejemplo:**

```bash
#!/bin/sh
echo "Running tests..."
npm test
```

---

### commit-msg

Se ejecuta al escribir el mensaje.

**¿Qué hace?**
- Validar formato del commit

---

### pre-push

Se ejecuta antes de hacer push.

**¿Qué hace?**
- Evitar subir código roto

---

## ⚙️ Cómo crear un hook

```bash
cd .git/hooks
touch pre-commit
chmod +x pre-commit
```

---

## 📌 Casos de uso

- Ejecutar tests
- Formatear código
- Validar commits

---

## ⚠️ Importante

- No se versionan por defecto
- Cada dev tiene los suyos

---

## 🧠 Pro tip

Se pueden manejar con herramientas como:
- Husky (Node.js)