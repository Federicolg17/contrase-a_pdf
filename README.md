# contrase-a_pdf
El presente proyecto es desarrollado con el propósito de generar una contraseña de seguridad a un conjunto de archivos pdf
🔐 PDF Password Protector

🚀 Descripción

PDF Password Protector es una herramienta Python que permite proteger múltiples archivos PDF con contraseña de manera automática. Ideal para procesar lotes de certificados, documentos confidenciales o cualquier colección de PDFs que requieran protección.

✨ Características principales

🔒 Protección masiva: Procesa todos los PDFs de una carpeta automáticamente
🛡️ Seguridad robusta: Utiliza encriptación R=4 con contraseñas de propietario y usuario
⚡ Procesamiento eficiente: Sobrescribe archivos directamente sin duplicados
🔄 Método alternativo: Incluye opción de procesamiento con archivos temporales
📋 Feedback detallado: Muestra el progreso y errores durante el proceso
🎯 Fácil configuración: Solo requiere modificar la ruta y contraseña

📋 Requisitos

Python 3.6 o superior
pikepdf library

🔧 Instalación

Clona el repositorio:
bash
git clone https://github.com/tu-usuario/pdf-password-protector.git
cd pdf-password-protector
Instala las dependencias:
bash
pip install pikepdf

🎯 Uso

Configura el script:
Modifica la variable password con tu contraseña deseada
Actualiza la ruta pdf_folder con la carpeta que contiene tus PDFs
Ejecuta el script:
bash
python pdf_protector.py

📁 Estructura de carpetas esperada

tu-proyecto/
├── pdf_protector.py
└── certificados/
    └── PDF/
        ├── documento1.pdf
        ├── documento2.pdf
        └── documento3.pdf
        
⚙️ Configuración

python
# Cambia estos valores según tus necesidades
password = "tu_contraseña_segura"
pdf_folder = "/ruta/a/tu/carpeta/de/pdfs"

🛠️ Métodos de procesamiento

El script incluye dos métodos de procesamiento:
Método 1: Sobrescritura directa (Por defecto)
Utiliza allow_overwriting_input=True
Más eficiente en memoria
Recomendado para la mayoría de casos
Método 2: Archivo temporal (Alternativo)
Crea un archivo temporal durante el proceso
Más seguro para archivos críticos
Descomenta las líneas correspondientes para usarlo

📊 Ejemplo de salida

Archivo 'certificado_juan.pdf' protegido con contraseña.
Archivo 'certificado_maria.pdf' protegido con contraseña.
Archivo 'certificado_carlos.pdf' protegido con contraseña.

✅ Procesamiento completado: 3 archivos protegidos

🔍 Casos de uso

Certificados académicos: Protege certificados de cursos o diplomas
Documentos corporativos: Asegura documentos confidenciales
Reportes financieros: Protege información sensible
Contratos y acuerdos: Añade seguridad a documentos legales

⚠️ Consideraciones importantes

Backup: Siempre realiza copias de seguridad antes de procesar archivos importantes
Contraseñas: Usa contraseñas seguras y guárdalas de forma segura
Permisos: Asegúrate de tener permisos de escritura en la carpeta objetivo
Encriptación: El nivel R=4 proporciona seguridad estándar para la mayoría de casos
