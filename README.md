# LaTeXTemplateTFG
## Español

Este repositorio contiene una plantilla LaTeX para el Trabajo de Fin de Grado de la Escuela Técnica de Ingeniería Informática (ETSInf) de la Universidad Politécnica de Valencia (UPV).

En ella se corrige un error relacionado con el entorno algorithm, utilizado para incorporar pseudocodigo, que impide que se compile correctamente el documento si se incluye un caption en el entorno.

Puedes encontrar la plantilla original en la web de la ETSInf (http://www.inf.upv.es/www/etsinf/wp-content/uploads/2017/06/U0724319.rar), información sobre diferentes plantillas y guías de estilo (https://www.inf.upv.es/www/etsinf/es/plantilla-tfg/) y otra información de interés (https://www.inf.upv.es/www/etsinf/es/category/secretaria/tfg/) como preguntas frecuentes [FAQ](https://www.inf.upv.es/www/etsinf/es/preguntas-frecuentes-faqs-tfg-tfm/).

Si ya dispones de la plantilla, únicamente hace falta que te descargues \tex\latex\tfgetsinf\tfgetsinf.cls, o en su defecto modificar dentro de ese documento la línea que declara el entorno de algorithm, eliminando la parte de name:

%Antes

\DeclareFloatingEnvironment[fileext=loa,listname=\listalgorithmname,name=\algorithmname]{algorithm}

%Después

\DeclareFloatingEnvironment[fileext=loa,listname=\listalgorithmname]{algorithm}

Además necesitas utilizar el comando \hrulefill entre \end{algorithmic} y \end{algorithm} para conseguir el estilo deseado.
  

## English

This repository contains a LaTeX template for degree's final project of ETSInf (UPV).

An error related to the algorithm enviroment, used to format pseudocode, it's fixed. You can find the original template in ETSInf's website (http://www.inf.upv.es/www/etsinf/wp-content/uploads/2017/06/U0724319.rar), more information related to the different templates  (https://www.inf.upv.es/www/etsinf/es/plantilla-tfg/) and general information about the final project (https://www.inf.upv.es/www/etsinf/es/category/secretaria/tfg/) cas the FAQ (https://www.inf.upv.es/www/etsinf/es/preguntas-frecuentes-faqs-tfg-tfm/).

If you have already the template the only file that has been modified is \tex\latex\tfgetsinf\tfgetsinf.cls. You can also modify your local copy where algorithm enviroment is modified, as you can se in the following lines:

%Before

\DeclareFloatingEnvironment[fileext=loa,listname=\listalgorithmname,name=\algorithmname]{algorithm}

%After

\DeclareFloatingEnvironment[fileext=loa,listname=\listalgorithmname]{algorithm}

Also you need to add the command \hrulefill between \end{algorithmic} and \end{algorithm} to achieve the desired style.
