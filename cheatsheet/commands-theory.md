# 🧠 Git Commands - Guía Completa (Teoría + Uso)

Este documento contiene una explicación completa de los comandos más importantes de Git, incluyendo:
- Qué hace cada comando
- Cómo funciona internamente
- Variantes
- Cuándo usarlo

---

# 📦 INICIALIZACIÓN Y CONFIGURACIÓN

## git init

```bash
git init
```

**¿Qué hace?**  
Inicializa un repositorio Git en el directorio actual.

**¿Cómo funciona internamente?**
- Crea la carpeta oculta `.git`
- Inicializa el historial vacío
- Define la rama principal (`main` o `master`)

**¿Cuándo usarlo?**
- Cuando empezás un proyecto desde cero

---

## git clone

```bash
git clone <url>
```

**¿Qué hace?**  
Clona un repositorio remoto en tu máquina.

**¿Cómo funciona internamente?**
- Descarga todo el historial del repo
- Configura el remoto `origin`
- Crea una copia completa

**Variantes:**
```bash
git clone -b <branch> <url>
git clone --depth 1 <url>
```

**¿Cuándo usarlo?**
- Cuando trabajás con un repo existente

---

## git remote

```bash
git remote -v
git remote add origin <url>
```

**¿Qué hace?**  
Gestiona repositorios remotos.

**¿Cómo funciona?**
- `origin` es un alias del repo remoto
- Permite vincular local ↔ remoto

---

# 📂 ESTADO Y CAMBIOS

## git status

```bash
git status
```

**¿Qué hace?**  
Muestra el estado actual del repositorio.

**Muestra:**
- Archivos modificados
- Archivos en staging
- Archivos sin trackear

---

## git diff

```bash
git diff
git diff rama1 rama2
```

**¿Qué hace?**  
Muestra diferencias entre archivos o ramas.

---

# ➕ STAGING

## git add

```bash
git add .
git add archivo.txt
```

**¿Qué hace?**  
Agrega archivos al staging area.

**Variantes:**
```bash
git add -p
```

---

## git reset (archivos)

```bash
git reset archivo.txt
```

**¿Qué hace?**  
Saca archivos del staging sin borrar cambios.

---

# 💾 COMMITS

## git commit

```bash
git commit -m "mensaje"
```

**¿Qué hace?**  
Guarda cambios en el historial.

**Variantes:**
```bash
git commit -am "mensaje"
```

---

## git log

```bash
git log
```

**¿Qué hace?**  
Muestra historial de commits.

**Variantes:**
```bash
git log --oneline
git log --graph --all
```

---

## git show

```bash
git show <hash>
```

**¿Qué hace?**  
Muestra detalles de un commit.

---

# 🌿 RAMAS

## git branch

```bash
git branch
git branch nueva-rama
```

**¿Qué hace?**  
Gestiona ramas.

---

## git checkout / switch

```bash
git checkout rama
```

```bash
git switch rama
```

**¿Qué hace?**  
Cambia de rama.

---

## git merge

```bash
git merge rama
```

**¿Qué hace?**  
Une ramas.

---

## git rebase

```bash
git rebase main
```

**¿Qué hace?**  
Reescribe el historial aplicando commits sobre otra rama.

---

# 🚀 REMOTO

## git push

```bash
git push
```

**¿Qué hace?**  
Sube cambios al remoto.

**Variantes:**
```bash
git push -u origin rama
git push -f
```

---

## git pull

```bash
git pull
```

**¿Qué hace?**  
Trae cambios y los mergea.

---

## git fetch

```bash
git fetch
```

**¿Qué hace?**  
Descarga cambios sin aplicarlos.

---

# ⏪ DESHACER CAMBIOS

## git reset

```bash
git reset --soft <hash>
git reset --hard <hash>
```

**¿Qué hace?**  
Mueve el HEAD.

---

## git revert

```bash
git revert <hash>
```

**¿Qué hace?**  
Deshace un commit creando uno nuevo.

---

## git reflog

```bash
git reflog
```

**¿Qué hace?**  
Muestra historial completo (incluye commits perdidos).

---

# 🧹 OTROS

## git stash

```bash
git stash
git stash pop
```

**¿Qué hace?**  
Guarda cambios temporalmente.

---

## git tag

```bash
git tag v1.0
```

**¿Qué hace?**  
Crea versiones del proyecto.

---

## git clean

```bash
git clean -fd
```

**¿Qué hace?**  
Elimina archivos no trackeados.