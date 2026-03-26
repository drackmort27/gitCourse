# 🔄 Git Workflows - Explicación Completa

Este documento explica los principales flujos de trabajo en Git, cómo funcionan y cuándo usar cada uno.

---

## 🌿 Feature Branch Workflow

### 📌 ¿Qué es?
Es el flujo más común. Cada funcionalidad se desarrolla en una rama separada.

### 🔄 Flujo paso a paso

```bash
git checkout -b feature/login
```

**¿Qué hace?**
- Crea una nueva rama
- Te mueve a esa rama

---

```bash
git add .
git commit -m "feat: login"
```

**¿Qué hace?**
- Guarda los cambios en la rama

---

```bash
git push -u origin feature/login
```

**¿Qué hace?**
- Sube la rama al remoto
- La deja trackeada

---

### 🔀 Pull Request

**¿Qué es?**
- Solicitud para mergear cambios a `main`

**¿Para qué sirve?**
- Code review
- Validación
- Discusión

---

### 📌 ¿Cuándo usarlo?
- Trabajo en equipo
- Desarrollo de features

---

## 👥 Git Flow

### 📌 ¿Qué es?
Un workflow más estructurado para proyectos grandes.

### 🌿 Ramas principales

- `main` → producción
- `develop` → desarrollo

### 🌱 Ramas auxiliares

- `feature/*`
- `release/*`
- `hotfix/*`

---

### 🔄 Ejemplo

```bash
git checkout develop
git checkout -b feature/pago
```

---

### 📌 ¿Cuándo usarlo?
- Equipos grandes
- Releases frecuentes

---

## 🔁 Forking Workflow

### 📌 ¿Qué es?
Cada dev trabaja sobre su propio fork.

---

### 🔄 Flujo

```bash
git clone <tu-fork>
git checkout -b feature
git push origin feature
```

---

### 📌 Pull Request
Se hace hacia el repo original.

---

### 📌 ¿Cuándo usarlo?
- Open source
- Proyectos públicos

---

## ⚖️ Comparación

| Workflow        | Uso principal        |
|----------------|---------------------|
| Feature Branch | Equipos chicos/medios |
| Git Flow       | Proyectos grandes    |
| Forking        | Open source         |