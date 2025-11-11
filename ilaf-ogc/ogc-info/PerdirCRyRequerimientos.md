### ¿Cómo perdir cambios y nuevos requerimientos en los estándares OGC?
#### Buscar el estándar correcto
Cuando un implementador o usuario necesita una determinada funcionalidad puede consultar la lista de estándares del OGC en http://www.opengeospatial.org/standards. Los estándares son documentos PDF que pueden venir acompañados de schemas XML (http://schemas.opengis.net/).
Ejemplo: La última versión del estándar OGC WMS (1.3.0 el dia que escribo estas líneas) que puede descargarse de: http://www.opengeospatial.org/standards/wms y sus esquemas de http://schemas.opengis.net/wms/

#### Introducir un nuevo requerimiento
En caso de que la versión actual no contemple alguna funcionalidad, es posible rellenar un formulario para solicitar un nuevo requerimiento (New Requirement http://portal.opengeospatial.org/public_ogc/change_request.php). Un ejemplo ficticio pero que alguna vez se ha debatido seria:
Title: Perfil unidimensional para WMS
Source: ILAF
Priority/Criticality: Major
Requirement Description: "Si la capa servida tiene valores continuos a lo largo del territorio, incluir la posibilidad de extraer un perfil unidimensional de esos datos en forma de gráfico".
Documents Affected: Web Map Service (WMS) Implementation Specification - v1.3.0 (06-042)
Consequences if not met: No puedo presentar un grafico de manera estándar

#### Introducir una petición de cambio
También es posible que se encuentre la funcionalidad pero no nos resulte adecuada o incluso que exista un error en la documentación o en los esquemas. En este caso se optará por rellenar un formulario de petición de cambio (Change Request). Un ejemplo que actualmente ser está considerando en el grupo de trabajo del WMS es:
Abstract Specification, Implementation Standard, or Best Practices: WMS
For OGC Standards, version of the Standard: 1.3.0
OGC Project Document number: 06-042
Title: Rectangular GetFeatureInfo
Source: ILAF
Category: C (Functional modification of feature)
Reason for change: Algunas veces, resulta difícil indicar las coordenadas de un píxel concreto cuando la capa presenta elementos puntuales muy pequeños.
Summary of change: En lugar de un punto, seria conveniente poder indicar las coordenadas de un rectángulo. el resultado de la consulta debe incluir todos los elementos que contiene ese rectángulo.
Consequences if not approved: Frecuentes mensajes de "no hay objetos" al no coincidir exactamente el punto solicitado con la coordenada del punto.
Clauses affected: 7.4 GetFeatureInfo

#### Observaciones
Aunque el sistema de entrada de requerimientos y peticiones de cambio se encuetra sólo en inglés, es posible introducir los textos en castellano. El personal de OGC pedirá ajuda a un miembro de ILAF para su traducción y consideración.