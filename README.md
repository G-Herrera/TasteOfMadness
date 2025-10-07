# TasteOfMadness
Este es el repositorio que contiene todo lo relaciando con el desarrollo de TasteOfMadness en Unreal Engine.

//Convencion y orden en los archivos

Estas tablas definen las convenciones de nombres que todo el equipo debe seguir en Taste of Madness.
El objetivo es que cualquier miembro pueda identificar un asset al instante, sin necesidad de abrirlo, 
y que la estructura del proyecto en Unreal Engine se mantenga clara y escalable.

Como leer las tablas

Prefijo: Codigo corto al inicio del nombre que indica el tipo de asset (ej: BP_ = Blueprint).

Ejemplo: Nombre sugerido aplicando la convencion.

Carpeta destino: Carpeta dentro del Content Browser donde debe guardarse el asset.

Descripcion: Explica brevemente el proposito del asset y que esperar de el.

Siguiendo estas reglas:

Los nombres seran consistentes y faciles de buscar.

Las carpetas estaran organizadas y separadas por funcion.

Cualquier desarrollador nuevo podra entender el proyecto rapidamente.

//Blueprints

| Prefijo  | Ejemplo             | Carpeta destino          | Descripcion                        |
| -------- | ------------------- | ------------------------ | ---------------------------------- |
| **BP\_** | `BP_OrderSystem`    | `Blueprints/Systems`     | Blueprint de sistema general       |
| **BP\_** | `BP_ClareCharacter` | `Characters/Clare`       | Personaje jugable o NPC            |
| **BP\_** | `BP_Food_Tomato`    | `Items/Food/Ingredients` | Consumible/Ingrediente interactivo |
| **BP\_** | `BP_Dish_Soup`      | `Items/Food/Dishes`      | Platillo terminado                 |
| **BP\_** | `BP_Item_Knife`     | `Items/Tools`            | Herramienta o utensilio            |

Widgets (UI)

| Prefijo   | Ejemplo   | Carpeta destino | Descripcion           |
| --------- | --------- | --------------- | --------------------- |
| **WBP\_** | `WBP_HUD` | `Blueprints/UI` | Widget Blueprint (UI) |

Animaciones

| Prefijo   | Ejemplo           | Carpeta destino    | Descripcion         |
| --------- | ----------------- | ------------------ | ------------------- |
| **A\_**   | `A_Clare_Idle`    | `Characters/Clare` | Animacion simple    |
| **AM\_**  | `AM_Clare_Attack` | `Characters/Clare` | Animation Montage   |
| **ABP\_** | `ABP_Clare`       | `Characters/Clare` | Animation Blueprint |

Materiales y texturas

| Prefijo  | Ejemplo           | Carpeta destino       | Descripcion                    |
| -------- | ----------------- | --------------------- | ------------------------------ |
| **M\_**  | `M_Wood`          | `Materials/Props`     | Material base                  |
| **MI\_** | `MI_Wood_Dirty`   | `Materials/Props`     | Material Instance              |
| **T\_**  | `T_Clare_Diffuse` | `Textures/Characters` | Textura (difuse, normal, etc.) |


Meshes

| Prefijo  | Ejemplo        | Carpeta destino    | Descripcion   |
| -------- | -------------- | ------------------ | ------------- |
| **S\_**  | `S_TableRound` | `Props/Static`     | Static Mesh   |
| **SK\_** | `SK_Clare`     | `Characters/Clare` | Skeletal Mesh |


Niveles y Camaras

| Prefijo | Ejemplo     | Carpeta destino       | Descripcion  |
| ------- | ----------- | --------------------- | ------------ |
| **L\_** | `L_Kitchen` | `Maps`                | Nivel (mapa) |
| **C\_** | `C_TopDown` | `Blueprints/Gameplay` | Camara       |


Audio

| Prefijo  | Ejemplo          | Carpeta destino | Descripcion               |
| -------- | ---------------- | --------------- | ------------------------- |
| **P\_**  | `P_BloodSplash`  | `FX`            | Particle System (Cascade) |
| **NS\_** | `NS_MadnessAura` | `FX`            | Niagara System            |

//FLUJO DE TRABAJO USANDO GITHUB DESKTOP Y CORRECTOS CAMBIOSO DENTRO DE UNREAL

--ACTUALIZAR EL PROYECTO ANTES DE TRABAJAR

`IMPORTANTE:ANTES DE EMPEZAR A TRABAJAR EN ALGO DENTRO DE UNREAL.`

1 Abres la applicacion de GitHub desktop si no la tienes abierta
2 Te aseguras de estar en la rama de develop
    Si no estas la seleccionas current branch --> choose a branch --> develop
3 Clic en Fetch origin
4 Clic en Repository --> pull (esto descarga la version mas reciente del proyecto)
5 Ya actualizado crea o cambiate a tu propia rama

--TRABAJAR DENTRO DE UNREAL ENGINE

`IMPORTANTE:CADA MIEMBRO DEBE TRABAJAR SOLO EN SU SUBNIVEL JAMAS SE MODIFICA EL MAINPERSISTENT.`
`NO TOCAR LOS NIVELES DE LOS OTROS MIEMBROS`
`CADA INTEGRANTE ES RESPONSABLE DE LA CORRECTA EJECUCION DE SU NIVEL, VERIFICAR ANTES DE SUBIR`

1 Abrir MainPersistent.umap
2 Ir al panel Levels dar doble click en tu nivel o con click derecho make current (se debe ver en negritas)
2.5 Puedes trabajar directamente en tu nivel buscandolo en el content browser y dandole doble click
3 Trabaja en lo que tengas que trabajar en tu nivel
4 Una vez hayas finalizado guardas tu nivel
5 CIERRA UNREAL antes de subir los cambios

--GUARDAR Y SUBIR MIS CAMBIOS

1 Ir a GitHub desktop
2 Veras tus cambios listados en la parte izquierda
3 Escribe el commit
4 Clic en commit
5 Hacer push origin

--MANTENER ACTUALIZADA TU RAMA AL DIA

1 En GitHub desktop ir a la rama develop
2 Click en fetch origin
3 Click en repository --> pull
4 Cambias a tu rama
5 Click en branch --> merge into current branch
    Seleccionas develop (esto actualiza tu rama con los cambios mas recientes del equipo)
6 Si UE te pide que resuelvas conflictos lo haces, guardas y vuelves a hacer commit

--ENVIAR TUS CAMBIOS A DEVELOP (PULL REQUEST)

1 Asegurate que desde tu rama hayas hecho el push origin
2 Click en branch --> view branch on GitHub
3 en la pagina del repo haz click en el boton verde "Compare & Pull Request"
4 Escribe un titulo claro y una descripcion
`IMPORTANTE:ASEGURATE QUE DIGA BASE:DEVELOP <-- COMPARE: NOMBREDETURAMA`
5 Click en create pull request

--LIMPIEZA DE RAMAS VIEJAS

1 Una vez que tu rama ya ha sido aprobada e integrada a develop vas a GitHub desktop
2 Con tu rama seleccionada click en branch --> delete branch
3 En el mensaje selecciona que igual la quieres eliminar del online si ya no se necesita.




