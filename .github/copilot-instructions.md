# Copilot Instructions for AI Coding Agents

## Descripción general del proyecto
Este repositorio parece estar en una fase inicial, con una estructura mínima: un archivo `test.txt` y una carpeta vacía `y/`. No se han encontrado archivos de configuración, documentación ni convenciones previas para agentes de IA.

## Convenciones y patrones actuales
- No existen convenciones específicas ni patrones de arquitectura definidos en el código base actual.
- No hay flujos de trabajo de desarrollo, scripts de construcción, pruebas ni integración continua configurados.
- No se detectan dependencias externas ni puntos de integración.

## Recomendaciones para agentes de IA
- Antes de agregar nuevas funcionalidades, consulta con el usuario sobre la estructura deseada, convenciones y tecnologías preferidas.
- Si se agregan archivos, sigue la organización actual y documenta cualquier decisión relevante en el README.md.
- Si se inicia una arquitectura, documenta los componentes principales y los flujos de datos en este archivo y en el README.md.
- Mantén las instrucciones concisas y actualizadas conforme evolucione el proyecto.

## Ejemplo de acción inicial
- Para agregar un nuevo módulo, crea una carpeta bajo la raíz y documenta su propósito en el README.md.
- Si se agregan scripts, incluye instrucciones de uso en comentarios y en el README.md.

## Archivos clave
- `.github/copilot-instructions.md`: Guía para agentes de IA (este archivo).
- `README.md`: Documentación general del proyecto (crear si es necesario).
- `test.txt`: Archivo de texto de ejemplo.
- `y/`: Carpeta vacía para futuros módulos o archivos.

---
Actualiza este archivo conforme se agreguen nuevas convenciones, flujos de trabajo o componentes relevantes.

import okhttp3.OkHttpClient;
import okhttp3.Request;
import okhttp3.Response;

public class WhatsAppAPIExample {
    public static void main(String[] args) throws Exception {
        OkHttpClient client = new OkHttpClient();
        Request request = new Request.Builder()
            .url("https://graph.facebook.com/v17.0/<tu-numero>/messages? 5526718926 access_token=<tu-230898>")
            .build();
        Response response = client.newCall(request).execute();
        System.out.println(response.body().string());
    }
}
