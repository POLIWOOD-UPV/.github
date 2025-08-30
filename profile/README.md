# 👋 Bienvenid@ a la organización de GitHub de POLIWOOD

Este repositorio es tu **punto de bienvenida**. Aquí aprenderás a configurar Git en tu máquina y a trabajar con nuestros repositorios de la organización.

---

## ⚙️ Configuración inicial de Git

### 🔧 Configuración de usuario y VSCode como editor
Ejecuta estos comandos en tu terminal:

```bash
git config --global user.name "<tu_nombre>"
git config --global user.email "<tu_correo>"
git config --global core.editor "code --wait"

git config --global diff.tool vscode
git config --global difftool.vscode.cmd 'code --wait --diff $LOCAL $REMOTE'
git config --global merge.tool vscode
git config --global mergetool.vscode.cmd 'code --wait --merge $REMOTE $LOCAL $BASE $MERGED'
```

### 🔍 Verificar o editar configuración
- Ver todo lo configurado:  
  ```bash
  git config --global --list
  ```
- Quitar un valor:  
  ```bash
  git config --global --unset <ITEM>
  ```
- Editar manualmente el archivo de configuración:  
  ```bash
  git config --global --edit
  ```

---

## 📂 Uso de GitHub

### 🔑 Acceso a un repositorio
Clona el repo que necesites. Ejemplo:

```bash
git clone https://github.com/POLIWOOD-UPV/salon-comic
```

O con un nombre de carpeta personalizado:

```bash
git clone https://github.com/POLIWOOD-UPV/salon-comic <nombre_carpeta>
```

---

### 🔄 Flujo básico de trabajo

1. Traer la última versión del código:
   ```bash
   git pull
   ```
2. Haz tus cambios (editar/crear archivos).
3. Añade los archivos al “stage”:
   ```bash
   git add <archivo>
   ```
4. Crea un commit con un mensaje claro:
   ```bash
   git commit -m "mensaje relevante"
   ```
   > 📝 El mensaje debe explicar lo que hiciste en **una frase breve**.  
   > Ejemplo: `Dockerfile actualizado con X docker`
5. Envía tus cambios al repositorio remoto:
   ```bash
   git push origin main
   ```

---

### 🕹️ Comandos útiles de control de cambios

- Ver estado rápido:  
  ```bash
  git status --short
  ```

- Ver historial gráfico resumido:  
  ```bash
  git log --oneline --all --graph
  ```

- Ver historial a través de interfaz gráfica:  
  ```bash
  gitk
  ```

---

## 📌 Notas finales
- Usa siempre mensajes de commit relevantes.  
- Antes de empezar a trabajar, haz siempre `git pull` para traer lo último.  
- Si tienes dudas, pregunta al equipo — la idea es que tod@s aprendamos.

---
## 🫂 Equipos 
Actualmente existe el equipo `PoliDevs`, este es el principal equipo de desarrollo de POLIWOOD.
---

✨ Bienvenid@ al equipo POLIWOOD 
