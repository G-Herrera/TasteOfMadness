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


Niveles y Cámaras

| Prefijo | Ejemplo     | Carpeta destino       | Descripcion  |
| ------- | ----------- | --------------------- | ------------ |
| **L\_** | `L_Kitchen` | `Maps`                | Nivel (mapa) |
| **C\_** | `C_TopDown` | `Blueprints/Gameplay` | Camara       |


Audio

| Prefijo  | Ejemplo          | Carpeta destino | Descripcion               |
| -------- | ---------------- | --------------- | ------------------------- |
| **P\_**  | `P_BloodSplash`  | `FX`            | Particle System (Cascade) |
| **NS\_** | `NS_MadnessAura` | `FX`            | Niagara System            |




