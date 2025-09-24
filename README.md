# PYTHON_BASES
Material del entrenamiento de programación en Python

# 🚀 Guía rápida: Git + GitHub con SSH

Este proyecto usa Git y GitHub con autenticación mediante **llaves SSH**.  
Aquí encontrarás un resumen de los pasos realizados y los comandos más útiles para trabajar con repositorios.

---

## 📌 Subir un repositorio local a GitHub (con SSH)

1. **Inicializar Git en el proyecto local**
```bash
git init
```

2. **Agregar archivos al área de staging**
```bash
git add .
```
👉 El punto (`.`) agrega todos los archivos de la carpeta.

3. **Crear el primer commit**
```bash
git commit -m "Primer commit"
```

4. **Configurar el remoto (usar SSH)**
```bash
git remote add origin git@github.com:henpv/PYTHON_BASES.git
```

5. **Verificar que el remoto quedó bien configurado**
```bash
git remote -v
```

6. **Renombrar la rama principal a `main` (recomendado)**
```bash
git branch -M main
```

7. **Subir los cambios al repositorio remoto**
```bash
git push -u origin main
```

---

## 📌 Comandos Git más útiles

### 🔄 Ver estado del repositorio
```bash
git status
```
👉 Muestra qué archivos han cambiado, cuáles están listos para commit y cuáles no.

---

### 📋 Ver historial de commits
```bash
git log --oneline
```
👉 Muestra el historial de commits en una sola línea por commit.

---

### ➕ Agregar archivos
```bash
git add archivo.txt
git add .
```
👉 Agrega un archivo específico o todos los archivos al staging area.

---

### 💾 Crear un commit
```bash
git commit -m "Mensaje descriptivo"
```
👉 Guarda los cambios en el historial del proyecto.

---

### ⬆️ Subir cambios al remoto
```bash
git push
```
👉 Sube los commits locales al repositorio remoto.

---

### ⬇️ Descargar cambios del remoto
```bash
git pull
```
👉 Descarga y aplica los cambios del repositorio remoto al local.

---

### 🔀 Crear y cambiar de ramas
```bash
git checkout -b nueva-rama
```
👉 Crea y mueve a una nueva rama.

```bash
git checkout main
```
👉 Cambia de vuelta a la rama principal.

---

### 🔄 Fusionar ramas
```bash
git merge nueva-rama
```
👉 Fusiona `nueva-rama` con la rama actual.

---

### 🗑️ Deshacer cambios (antes de commit)
```bash
git restore archivo.txt
```
👉 Revierte los cambios de un archivo antes de agregarlos al commit.

---

## ✅ Recomendaciones
- Usar mensajes de commit claros y descriptivos.  
- Mantener el repo sincronizado con `git pull` antes de trabajar.  
- Trabajar en ramas para nuevas funciones y luego hacer `merge`.  
- Proteger la llave privada SSH (no compartirla nunca).

---
