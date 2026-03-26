# 📦 Git Submodules - Explicación Completa

Permiten incluir un repositorio dentro de otro.

---

## 📌 ¿Qué es un submodule?

Es un repo externo referenciado dentro de otro repo.

---

## ➕ Agregar submodule

```bash
git submodule add <repo>
```

**¿Qué hace?**
- Agrega un repo dentro del proyecto
- Guarda referencia a un commit específico

---

## 📥 Clonar con submodules

```bash
git clone --recurse-submodules <repo>
```

**¿Qué hace?**
- Clona repo principal + submodules

---

## 🔄 Inicializar submodules

```bash
git submodule update --init --recursive
```

**¿Qué hace?**
- Descarga contenido de submodules

---

## 🔁 Actualizar

```bash
git submodule update --remote
```

---

## 📌 ¿Cuándo usarlo?

- Librerías externas
- Repos compartidos

---

## ⚠️ Problemas comunes

- Quedan desactualizados
- Manejo más complejo

---

## 🧠 Alternativas

- Monorepo
- Package managers