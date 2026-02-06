# ¡Hola! Bienvenido al Github de Possumus

Para crear un nuevo repositorio o realizar algún otro tipo de cambio que requiera de permisos especiales, solicitalo en el Team de Staff etiquetando a Andrés Gomez/Mario Cuevas/Javier Valdivieso.

## Repositorios

Los repositorios siguen el siguiente esquema de nombrado:

### Repositorios de clientes

`client-{client-name}-{project-name}-{repo-contents}`

Ejemplos: 

`client-biotech-helpdesk-front` es un repositorio de cliente externo, siendo el cliente Biotech, el proyecto Help Desk, conteniendo el repo el frontend del proyecto.
`client-superapps-weather-android` es un repositorio de cliente externo, siendo el cliente Superapps, el proyecto Weather, conteniendo el repo la aplicación Android.

### Repositorios internos

`internal-{repo-contents}`

### Repositorios de productos internos

`internal-product-{product-name}-{repo-contents}`

Ejemplos:

`internal-product-paaxio-portal-ui`es un repositorio de producto interno, siendo el producto Paax.io, conteniendo el repo el portal UI.

## Acceso a Github y permisos sobre repositorios

### Colaboradores Internos

En el caso de colaboradores internos, deben ser invitados a la organización utilizando su cuenta de Github personal (u otra cuenta que se haya creado, en caso que no quiera utilizar la personal). Una vez aceptada la 
invitación, Github solicitará la vinculación con el SSO de Possumus, quedando así vinculada la cuenta de Github a su identidad en Possumus.

El control de permisos se hace mediante equipos (Teams) de Github, sincronizados con grupos en Microsoft Entra ID. Por ello, para poder acceder a los repositorios correspondientes, la cuenta de Possumus del colaborador debe estar asignada al grupo correspondiente a su equipo en Microsoft Entra ID.

#### Ejemplo

Si el dev Juan Perez (`juan.perez@possumus.tech`) necesita accesos al repositorio `client-superapps-weather-android`, los pasos son:

1- Invitar a Juan Perez a la organización en Github con su cuenta personal (ej: `juanperez_1990`)

2- Juan Perez acepta la invitación y Github le solicita la vinculación con su cuenta de Possumus, `juan.perez@possumus.tech`

3- Para poder ver el repositorio `client-superapps-weather-android`, Juan debe ser agregado al grupo de EntraID correspondiente a su rol en el proyecto en cuestión (ej: `DEVs-SuperApps`, `PMPO-SuperApps`). El proceso de asignación a un grupo y su reflejo en los permisos de Github puede tardar más de 30 minutos.

*NOTA:* El paso 3 puede hacerse sin necesidad de ejecutar previamente pasos anteriores.

### Colaboradores Externos

En el caso de colaboradores externos, deben ser invitados a la organización como EXTERNOS y se deben otorgar luego los permisos corrrespondientes a los repositorios a los que necesite acceso.
