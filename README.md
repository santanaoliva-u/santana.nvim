### **Guía Completa para la Instalación de Neovim Configurado: `santana.nvim`**

---

## 🛠️ **Requisitos Previos**

Antes de comenzar con la instalación, asegúrate de tener lo siguiente:

- **Neovim** >= **0.9.0** (debe estar compilado con **LuaJIT**).
- **Git** >= **2.19.0** (para soporte de clones parciales).
- [LazyVim](https://www.lazyvim.org/).
- Un [Nerd Font](https://www.nerdfonts.com/) (v3.0 o superior) **_(opcional, pero necesario para mostrar algunos íconos)_**.
- [lazygit](https://github.com/jesseduffield/lazygit) **_(opcional)_**.
- Un compilador de **C** para `nvim-treesitter`. Consulta [aquí](https://github.com/nvim-treesitter/nvim-treesitter#requirements).
- Para [telescope.nvim](https://github.com/nvim-telescope/telescope.nvim) **_(opcional)_**:
  - **live grep**: [ripgrep](https://github.com/BurntSushi/ripgrep).
  - **find files**: [fd](https://github.com/sharkdp/fd).
- Un terminal que soporte colores verdaderos y _undercurl_:
  - [kitty](https://github.com/kovidgoyal/kitty) **_(Linux & macOS)_**.
  - [wezterm](https://github.com/wez/wezterm) **_(Linux, macOS & Windows)_**.
  - [alacritty](https://github.com/alacritty/alacritty) **_(Linux, macOS & Windows)_**.
  - [iTerm2](https://iterm2.com/) **_(macOS)_**.
- [Solarized Osaka](https://github.com/santanaoliva-u/solarized-osaka.nvim).

---

## 📦 **Pasos de Instalación**

### 1. **Instalar Neovim**

Si aún no tienes Neovim instalado, sigue estos pasos:

- **Para Ubuntu/Debian:**

  ```bash
  sudo apt update
  sudo apt install neovim
  ```

- **Para Fedora:**

  ```bash
  sudo dnf install neovim
  ```

- **Para Arch Linux:**

  ```bash
  sudo pacman -S neovim
  ```

- **Para macOS usando Homebrew:**

  ```bash
  brew install neovim
  ```

- **Para Windows:**
  Descarga el instalador desde el [sitio oficial de Neovim](https://neovim.io/) y sigue las instrucciones.

### 2. **Clonar el Repositorio de Configuración**

Clona tu repositorio de configuración `santana.nvim` en el directorio de configuración de Neovim.

```bash
git clone https://github.com/santanaoliva-u/santana.nvim ~/.config/nvim
```

### 3. **Instalar los Plugins**

Tu configuración de Neovim utiliza `LazyVim` para la gestión de plugins. Sigue estos pasos para instalar los plugins necesarios:

1. **Abrir Neovim:**

   ```bash
   nvim
   ```

2. **Ejecutar el Comando de Instalación de Plugins:**
   Una vez en Neovim, ejecuta:

   ```vim
   :Lazy install
   ```

   - **Explicación:**
     - `:Lazy install`: Comando para instalar todos los plugins definidos en tu configuración usando `LazyVim`.

### 4. **Configurar Plugins Adicionales**

Si tu configuración de Neovim requiere plugins adicionales o configuraciones específicas, sigue las instrucciones en el `README.md` del repositorio.

1. **Revisar el `README.md`:**
   Abre el archivo `README.md` en el repositorio para cualquier instrucción específica de configuración.

2. **Instalar Dependencias de Plugins:**
   Algunos plugins pueden requerir dependencias externas. Instala cualquier dependencia siguiendo las instrucciones del `README.md`.

### 5. **Verificar la Instalación**

Para asegurarte de que todo está funcionando correctamente:

1. **Abrir Neovim:**

   ```bash
   nvim
   ```

2. **Verificar los Plugins Instalados:**
   Ejecuta el comando:

   ```vim
   :Lazy status
   ```

   - **Explicación:**
     - `:Lazy status`: Muestra el estado de los plugins instalados.

3. **Probar Configuraciones:**
   Navega por tu configuración para asegurarte de que todos los ajustes y plugins están funcionando como se espera.

---

# 🎨 **Instalación de Temas en Neovim**

Sigue estos pasos para instalar el tema `solarized-osaka.nvim` en Neovim:

1. **Clonar el Repositorio del Tema y Seguir sus Instrucciones:**

   [Instrucciones de instalación del tema](https://github.com/santanaoliva-u/solarized-osaka.nvim)

---

## 🔧 **Resolución de Problemas**

Si encuentras problemas durante la instalación, aquí algunos pasos para solucionarlos:

1. **Revisar los Logs de Neovim:**

   - Abre Neovim y ejecuta:
     ```vim
     :messages
     ```
   - Revisa los mensajes para cualquier error relacionado con la carga de plugins o configuraciones.

2. **Verificar la Configuración de `LazyVim`:**

   - Asegúrate de que `LazyVim` esté configurado correctamente en tu archivo `init.lua`.

3. **Consultar la Documentación:**

   - Revisa la documentación de los plugins y `LazyVim` para posibles problemas conocidos y soluciones.

4. **Buscar Ayuda en la Comunidad:**
   - Consulta foros y comunidades como Reddit, Stack Overflow o los canales de soporte de los plugins que estés usando.

---
