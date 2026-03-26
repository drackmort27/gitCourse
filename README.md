# 📦 Git Notes & Cheat Sheet

![Git](https://img.shields.io/badge/Git-Version%20Control-orange)
![Level](https://img.shields.io/badge/Level-Basic%20to%20Advanced-blue)

Repositorio con teoría, comandos y prácticas reales de Git.

---

## 📚 Contenido

- 📘 [Teoría](docs/theory.md)
- 🔄 [Workflows](docs/workflows.md)
- 🧠 [Cheat Sheet](cheatsheet/commands.md)
- 🧪 [Ejemplo](examples/basic-flow.md)
- ⚙️ [Hooks](advanced/hooks.md)
- 📦 [Submodules](advanced/submodules.md)
- 🚀 [CI/CD](advanced/cicd.md)

---

## 🚀 Flujo básico

```bash
git clone <repo>
git checkout -b feature/nueva-funcionalidad
git add .
git commit -m "feat: nueva funcionalidad"
git push -u origin feature/nueva-funcionalidad