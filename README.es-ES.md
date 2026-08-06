

# ⚡ Fooocus Compatible con RTX 50-Series (Versión Portátil)

## 🧠 Configuración sin complicaciones para usuarios de RTX 5080 / 5090

[Fooocus](https://github.com/lllyasviel/Fooocus) es una de las mejores interfaces de usuario para Stable Diffusion, pero no es compatible directamente con **GPUs de la serie RTX 50** (como la 5080 o 5090) debido a las **versiones más recientes de CUDA (12.8+)**.

Este repositorio soluciona ese problema al incluir:

- ✅ Una versión parcheada de PyTorch compatible con CUDA 12.8
- ✅ Todas las dependencias necesarias
- ✅ Python integrado (no es necesario instalar Python a nivel global)
- ✅ Lanzador `.bat` listo para usar

---

## ✅ Características

- Totalmente autocontenido y portátil (sin cambios en PATH)
- Funciona sin configuración previa en GPUs RTX 5080 / 5090
- Velocidades de iteración rápidas en GPUs modernas
- Soporta la descarga de modelos adicionales
- Funciona sin conexión y es portátil: ideal para entornos aislados (air-gapped)

---

Clonar e instalar localmente

```bash
git clone https://github.com/alibakhtiari2/fooocusrtx508090.git
cd fooocusrtx508090

Luego ejecuta:
install.bat

Esto hará lo siguiente:
Instalar pip en el Python integrado
Instalar PyTorch Nightly (con soporte para CUDA 12.8)
Instalar todas las dependencias desde requirements_versions.txt
Generar run.bat para iniciar Fooocus

⚠️ Nota: Ignora las advertencias amarillas como "pip not in PATH" — esto utiliza Python integrado y no se requiere configuración global.

🕒 Tiempo de configuración: ~5–10 minutos dependiendo de tu conexión.

🖼️ Agregar o actualizar modelos
Para agregar modelos personalizados:
Descarga modelos .safetensors o .ckpt desde Civitai o Hugging Face

Colócalos dentro del siguiente directorio:
Fooocus\models\checkpoints\
Ahora podrás seleccionarlos en la interfaz de Fooocus después de iniciar la aplicación.

🧪 Hardware probado
Esta versión ha sido probada y funciona en:

✅ NVIDIA RTX 5080

✅ NVIDIA RTX 5090

Rendimiento de alta velocidad y compatibilidad total confirmados.

🚀 Cómo ejecutar
Una vez completada la configuración, simplemente ejecuta:
run.bat
Esto inicia la interfaz web de Fooocus utilizando el entorno de ejecución de Python integrado y la compilación compatible de CUDA.

🙏 Créditos
Proyecto original: Fooocus por lllyasviel

Modificado y empaquetado por: Ali Bakhtiari alibakhtiari2@gmail.com

⚖️ Licencia y aviso de uso
Este repositorio se proporciona con fines de compatibilidad y educativos.

El código está bajo la Licencia MIT (de Fooocus)

Los modelos y compilaciones de tiempo de ejecución están bajo sus respectivas licencias:

PyTorch: Licencia estilo BSD

SDXL y derivados: Licencia CreativeML Open RAIL-M

Eres responsable de cumplir con las reglas de licencia y uso al distribuir o modificar modelos.
