# Creando una web en github

Estoy intentando crear una web en github. El objetivo sería una web mejor que la web personal upv. Y a ser posible con un blog en el que den ganas de escribir. Para ello estoy siguiendo los siguientes tutoriales:

- https://rstudio.github.io/distill/
- https://rstudio.github.io/distill/website.html
- https://rstudio.github.io/distill/publish_website.html#github-pages

Los pasos que he seguido para crear la web en github son:

1. Instalar Distill en RStudio. 

   - `devtools::install_github("rstudio/distill")`

1. Crear un repositorio en github "algarsal.github.io" que se corresponde con la web de github. 
3. Crear un repositorio en github "algarsal-web" aunque no sé si es necesario, aunque creo que sí. 

4. Clonar los dos repositorios en mi ordenador. 

   - `git clone https://github.com/algarsal/algarsal.github.io`
   - `git clone https://github.com/algarsal/algarsal-web`

5. Empezar a escribir este recordatorio en el Readme de algarsal-web.

1. Crear un proyecto (new project) de RStudio de página web de distill (Distill website) eligiendo la carpeta "algarsal.github.io". Se crean un montón de archivos. Commit y Push. 
    . Al abrir la web no funciona. 

6. Crear otro proyecto de blog de distill (Distill blog), eligiendo la carpeta "algarsal.github.io/blog" para crear un blog. 

   - Para actualizar el blog es necesario "Build" y "Build website" en el proyecto del blog. 
   - Para actualizar la web, lo mismo pero en el proyecto de la web. 
   - Los commits se pueden hacer desde cualquiera de los dos. 
   
7. Importante, en ambos archivos "_site.yml" poner 
`output_dir: "."`

9. Arreglar los links de ambos "_site.yml" para que coincidan. 
    - En el del blog, poner ../index.html para el principal.
    - En el principal, poner blog/index.html para el blog. 

