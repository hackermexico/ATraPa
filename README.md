# ATraPa

**Analizador de Tráfico Pasivo** (Passive Traffic Analyzer)

## Descripción

ATraPa nace con la intención de analizar tráfico y comparar diferentes capturas buscando conexiones sospechosas y dando algunos datos sobre ellas, como:

- La cantidad de datos de ida y vuelta que han intercambiado
- Resoluciones DNS
- Puertos y protocolos que han usado en la comunicación
- Número de veces que han establecido la comunicación
- Geolocalización de la IP implicada
- Y algunas cosas más

## Requisitos

- Sistema operativo: Ubuntu, Kali Linux (probado)
- Herramientas necesarias: `tcpdump`, `awk`, `grep`, `sed`
- Permisos de administrador para captura de tráfico

## Instalación

1. Descarga el archivo `ATraPa.sh` o copia su contenido en un archivo de texto
2. Dale permisos de ejecución: `chmod +x ATraPa.sh`
3. Ejecuta: `./ATraPa.sh`
4. Sigue las instrucciones en pantalla

## Uso

### Funcionalidades principales:

1. **Capturar tráfico para analizarlo** - Realiza una captura en tiempo real
2. **Analizar una captura existente** - Procesa archivos .cap/.pcap existentes
3. **Comparar 2 capturas** - Compara dos archivos de captura
4. **Hacer 2 capturas y compararlas** - Automatiza el proceso completo

### Importante:

⚠️ **CUANDO VAYAS A REALIZAR LAS CAPTURAS, ES IMPORTANTE NO ABRIR NADA EN EL DISPOSITIVO QUE PROVOQUE TRÁFICO (navegadores web, programas P2P, etc.)**

## Estructura del proyecto

```
ATraPa/
├── ATraPa.sh          # Script principal
├── capturas/          # Directorio para archivos de captura (se crea automáticamente)
└── datos/            # Directorio para datos temporales (se crea automáticamente)
```

## Estado del proyecto

Este proyecto lleva tiempo sin mantenimiento activo y no está completamente depurado. Ha sido probado principalmente en Ubuntu y Kali Linux.

## Contribuciones

Las mejoras y correcciones son bienvenidas. Algunos aspectos que necesitan atención:

- Validación mejorada de entrada de usuario
- Manejo de errores más robusto  
- Documentación adicional
- Pruebas en más distribuciones

## Autor

- **Javierbu** (javierbu@gmail.com) - Mayo 2015
- Colaborador: **Ivanuco**