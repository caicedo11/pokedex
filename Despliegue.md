# TUTORIAL PASO A PASO DEL DESPLIEGUE EN LA NUBE AZURE (STATIC WEB APPS)

A continuación le detallamos el procedimiento completo paso a paso para el despliegue y publicación de la aplicación **PokeDex** en la nube pública de **Microsoft Azure** utilizando el servicio **Azure Static Web Apps**.

**Paso a Paso para el Despliegue**

**Paso 1: Creación del recurso de Aplicación Web Estática**

1.  Iniciar sesión en el portal de Azure:  https://portal.azure.com 
    
2.  En la barra de búsqueda superior, buscar y seleccionar **Static Web Apps** (Aplicaciones web estáticas).
    
3.  Hacer clic en el botón **+ Crear** para iniciar el asistente de configuración.
    

**Paso 2: Configuración de Detalles del Proyecto**

1.  **Suscripción:** Seleccionar la suscripción activa.
    
2.  **Grupo de recursos:**  rg-PokeDex-prod-po.
    
3.  **Región de hospedaje:** Global.
    
4.  **Detalles de la aplicación web estática:**
    
    -   **Nombre:** app-PokeDex-web-po
        
    -   **Plan de hospedaje / Tipo de plan:** Seleccionamos **Gratis**.
        
**Paso 3: Configuración de la Implementación (Origen GitHub)**

1.  En la sección **Detalles de la implementación**, marcar el origen como **GitHub** y verificar la cuenta vinculada en mi caso es **caicedo11.**
    

**Paso 4: Detalles de Compilación** 

1.  En **Valores preestablecidos de compilación**, seleccionar **Angular** (detectado automáticamente).
    
2.  Configurar las rutas del proyecto:
    
    **Ubicación de la aplicación (App location):**  "/"
        
    **Ubicación de la API (Api location):** (Dejar en blanco)
        
      **Ubicación de salida (Output location):** dist/pokedex-angular
        

### **Paso 5: Vinculación con el Repositorio**

1.  Seleccionar los datos específicos del repositorio en GitHub:
    
    -   **Organización:** caicedo11
        
    -   **Repositorio:** pokedex
        
    -   **Rama (Branch):** main
        

**Paso 6: Revisión y Creación**

1.  Hacer clic en la pestaña **Revisar y crear** para validar que todos los parámetros técnicos y de compilación estén correctos.
    
2.  Hacer clic en el botón **Crear**. Azure generará automáticamente el recurso y configurará el archivo de flujo de trabajo de GitHub Actions en el repositorio.
   

**Paso 7: Verificación de la URL Pública y Seguridad**

1.  Al finalizar la implementación, iremos al recurso creado en el panel de Azure.
    
2.  En la sección de información general, copiaremos la URL del **Dominio predeterminado** https://red-desert-0c23bc310.2.azurestaticapps.net
    
3.  Aqui ya es el paso final en el cual verificamos si la url de verdad cargo.
    

