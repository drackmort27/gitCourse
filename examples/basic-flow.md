# 🧪 Flujo Básico de Trabajo en Git

Este ejemplo muestra el flujo típico desde clonar un repo hasta hacer un merge.

---

## 1. Clonar repositorio

```bash
git clone <url>
```

**¿Qué hace?**
- Descarga el repo completo
- Configura `origin`

---

## 2. Crear una rama

```bash
git checkout -b feature/test
```

**¿Qué hace?**
- Crea una rama nueva
- Cambia a esa rama

---

## 3. Hacer cambios

(editás archivos)

---

## 4. Agregar cambios

```bash
git add .
```

**¿Qué hace?**
- Prepara cambios para commit

---

## 5. Crear commit

```bash
git commit -m "feat: test"
```

**¿Qué hace?**
- Guarda cambios en historial

---

## 6. Subir cambios

```bash
git push -u origin feature/test
```

**¿Qué hace?**
- Sube la rama al remoto

---

## 7. Crear Pull Request

**¿Qué hace?**
- Permite revisar código
- Integrar cambios a `main`

---

## 8. Merge

```bash
git checkout main
git merge feature/test
```

**¿Qué hace?**
- Integra la funcionalidad

---

## 📌 Flujo resumido

```bash
git clone
git checkout -b feature
git add .
git commit
git push
PR → merge
```