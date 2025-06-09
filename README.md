# 🖥️ pop-electron

Aplicación de escritorio construida con [Electron](https://www.electronjs.org/) que encapsula el sitio oficial de la UTN Facultad Regional Villa María:  
🌐 [https://www.frvm.utn.edu.ar](https://www.frvm.utn.edu.ar)

---

## 📦 Requisitos

Antes de comenzar, asegurate de tener instalado:

- [Node.js](https://nodejs.org/) (versión 16 o superior recomendada)
- [npm](https://www.npmjs.com/) (viene con Node)
- [git](https://git-scm.com/)
- (opcional) [electron-builder](https://www.electron.build/) para empaquetar la app

---

## 🚀 Cómo ejecutar el proyecto

### 1. Clonar el repositorio

```bash
git clone https://github.com/geruvenier/pop-electron.git
cd pop-electron
```

### 2. Instalar dependencias

```bash
npm install
```

### 3. Ejecutar en modo desarrollo

```bash
npm start
```

Se abrirá una ventana que muestra el sitio web en modo aplicación de escritorio.

---

## 🛠 Estructura del proyecto

```
pop-electron/
├── main.js            # Proceso principal de Electron
├── package.json       # Configuración del proyecto y dependencias
├── icon.png           # Icono de la app (usado al empaquetar)
├── .gitignore
└── README.md
```

---

## ⚙️ Scripts disponibles

En el archivo `package.json` tenés los siguientes scripts configurados:

| Comando         | Descripción                                |
|----------------|---------------------------------------------|
| `npm start`     | Ejecuta la app en modo desarrollo          |
| `npm run pack`  | Empaqueta la app sin generar instalador    |
| `npm run dist`  | Compila la app y genera un instalador      |

---

## 🧪 Compilar la app

### Para empaquetar (sin instalador):

```bash
npm run pack
```

### Para generar un instalador:

```bash
npm run dist
```

Esto generará:

- En **macOS**: un archivo `.dmg`
- En **Windows**: un `.exe` (solo desde Windows)
- En **Linux** (si lo configurás): `.AppImage`, `.deb`, etc.

Los archivos compilados se almacenan en la carpeta `dist/`.

---

## ⚠️ Nota para usuarios de macOS

Electron no puede compilar directamente a Windows desde macOS, a menos que tengas instalado `wine`. Para builds multiplataforma recomendamos:

- Usar una VM con Windows (VirtualBox, VMware, Parallels, etc.)
- Usar GitHub Actions para automatizar builds en cada sistema operativo

---

## 📜 Licencia

Este proyecto está bajo la licencia MIT. Ver archivo `LICENSE` para más detalles.

---

## 👨‍💻 Autor

**Gerardo Venier**  
📧 [geruvenier@gmail.com](mailto:geruvenier@gmail.com)  

---
