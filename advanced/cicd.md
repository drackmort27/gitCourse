# 🚀 CI/CD - Integración y Despliegue Continuo

---

## 📌 ¿Qué es CI/CD?

### CI (Continuous Integration)
Automatiza:
- Build
- Test

### CD (Continuous Delivery/Deployment)
Automatiza:
- Deploy

---

## 🔄 Flujo típico

1. Hacés push
2. Se dispara pipeline
3. Corre build
4. Corre tests
5. Deploy

---

## ⚙️ Ejemplo con GitHub Actions

Archivo:

```
.github/workflows/ci.yml
```

---

```yaml
name: CI

on:
  push:
    branches: [main]

jobs:
  build:
    runs-on: ubuntu-latest

    steps:
      - name: Checkout repo
        uses: actions/checkout@v3

      - name: Run tests
        run: echo "Running tests..."
```

---

## 🔍 Explicación

**on: push**
- Ejecuta pipeline al hacer push

**jobs**
- Define tareas

**steps**
- Acciones dentro del job

---

## 📌 ¿Qué hace esto?**

- Clona repo
- Ejecuta comandos
- Automatiza validación

---

## 📌 ¿Cuándo usar CI/CD?**

- Siempre en proyectos reales
- Para evitar errores en producción

---

## ⚠️ Beneficios

- Automatización
- Menos errores
- Deploy rápido

---

## 🧠 Ejemplos reales

- Test automático
- Build Docker
- Deploy a servidor

---

## 🚀 Ejemplo más avanzado

```yaml
- name: Build Docker
  run: docker build -t app .

- name: Deploy
  run: echo "Deploying..."
```