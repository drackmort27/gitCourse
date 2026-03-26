# 🚀 CI/CD con Git

## 🧠 ¿Qué es?

Automatización de:
- Build
- Test
- Deploy

---

## 🔄 Flujo

1. Push
2. Pipeline corre
3. Tests
4. Deploy

---

## 🛠️ Ejemplo (GitHub Actions)

.github/workflows/ci.yml

```yaml
name: CI

on: [push]

jobs:
  build:
    runs-on: ubuntu-latest

    steps:
      - uses: actions/checkout@v3
      - run: echo "Running tests..."