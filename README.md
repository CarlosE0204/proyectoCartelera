# Proyecto de Cartelera de películas 
##### Dentro del presente git se puede visualizar un proyecto con relación a la presentación de peliculas. En el proyeco se presenta un diseño dinamico para el usuario. El cual en un inicio tiene una pantalla de login en el cual se piden ciertos datos como son el correo y la contraseña.
Después de ingresar al login este mostrará la pantalla principal en la cual se podrá visualizar 1 dashboard, una barra de menu en la parte superior la cual contiene el nombre del usuario logueado, y la foto de perfil.
En el dashboard se puede notar botones que estan direccionados a hacer ciertas acciones las cuales son Agregar usuario, Editar perfil, Agregar pelicula, los cuales son botones que tienen funcionalidades de servicio directamente con la API que habia sido creada en un inicio.

### Al momento de iniciar la pagina este muestra un pantalla de inicio de sesión en la cuale pide una usuario y contraseña. 
#### Por tanto en este apartado se realizó una pantalla exclusiva para este el cual esta hecho en html con el sigueinte código.

![image](https://github.com/user-attachments/assets/b511e538-4558-4c05-9720-a9c6d2723ebd)
##### El cual es validado con métodos que han sido creados en el typescript 
![image](https://github.com/user-attachments/assets/dbe52028-fe65-4edb-892f-dbcd61472611)
##### Dentro de método se validan los datos entrantes, hace un servicio HTTP en la cual una vez validado y que este registrado ingresara ala pantalla de home o pantalla principal en donde se presentara la información del usuario que inicio sesion, asi mismo los botones que servirán para acer acciones y una tabla en la que se visualizaran las películas.
### -> Pantalla Login 
![image](https://github.com/user-attachments/assets/09d76ce1-cf43-488f-ba56-05b09ad9f314)
#### Validando usuario
![image](https://github.com/user-attachments/assets/8d7e56a4-70a9-4226-93c0-1020a6e8ceb8)

#### Una vez validado el usuario se dirige a la pantalla de home
![image](https://github.com/user-attachments/assets/10e5336d-3d3f-41de-888e-c05519e07b83)

--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
## -> Pantalla Principal

#### Como inicio en la barra superior se muestran 2 datos las cuales son el nombre y su foto de perfil del usuario que ha iniciado sesion. Por tanto en el codigo que ve de la siguiente manera. 

![image](https://github.com/user-attachments/assets/de9532a7-e751-4dcb-a950-9a4a8f361711)

##### En donde se hacen consultas a la API por medio de un servicio con el cual obtendremos el nombre y la foto de perfil. Además de mencionar que en la foto de perfil se pueden ver ciertas acciones que puede hacer un usuario las cuales son 
![image](https://github.com/user-attachments/assets/de8c10d6-f6b8-4096-a49e-1c97698be0f6)

-----------------------------------------------------------------------------------------

#### * Mi perfil la cual tiene funcionalidad ya que en el typescript se realzia un método el cual tiene de nombre mi perfil la cual muestra con un dialog la información del usuario 
![image](https://github.com/user-attachments/assets/85ebec4d-6e87-48ea-a3bc-396d6fae861d)

![image](https://github.com/user-attachments/assets/b2a80d5d-ae56-4e68-895c-a3965039934d)

##### En codigo el dialog se realizo de la siguiete manera.
![image](https://github.com/user-attachments/assets/c1e2006f-ddc3-4a3e-b232-09117e615ac1)

-----------------------------------------------------------------------------------------
#### * Eliminar perfil la cuales tiene función en el typescript  
![image](https://github.com/user-attachments/assets/bb87fd60-a1d2-4b4e-a315-04143a85bdfc)
![image](https://github.com/user-attachments/assets/d137aace-3744-4e89-b45a-7b51f1f15c0a)

##### En el codigo del dialog de eliminar perfil
![image](https://github.com/user-attachments/assets/1d39834c-31b9-46ee-adc3-e03d67316304)

##### En el codigo muestra que cuando quiera eliminar la cuenta cuenta con 2 botones por tanto tendra que ingresar su contraseña y que este será validado en cuanto este se valide se eliminará.
![image](https://github.com/user-attachments/assets/ac3f3bd8-b947-45ec-929f-b13fb58854e6)

-----------------------------------------------------------------------------------------

##### * Enseguida esta el boton de cerrar sesión la cual regresará a el login. 
![image](https://github.com/user-attachments/assets/ea90e16d-72f6-4528-9e66-a9d0d36067e7)

![image](https://github.com/user-attachments/assets/b51b9c3a-3ed3-4370-9c04-a4149981dab9)

-----------------------------------------------------------------------------------------
### -> Dashboard
![image](https://github.com/user-attachments/assets/3816bd19-b7cf-486b-b779-7d2290283d3c)

#### En el dashboard se tienen botones los cuales son Editar perfil, Agregar usuario, Agregar peliculas y cerrar sesión.
![image](https://github.com/user-attachments/assets/fd3eaada-16e2-4570-9c81-9937694e8d49)

-------------------------------------------------------------------------------------------
#### * Editar perfil
##### En el botón de Editar perfil se realiza por medio de una pantlla que tiene un formulario en la que se muestran los datos como nombre, foto de perfil, etc. 
![image](https://github.com/user-attachments/assets/a8a040c6-9945-4705-8fd0-8ae98ebae057)
##### Para que pueda hacer un cambio es necesario que tenga un servicio el cual esta iniciado en el typescript 
![image](https://github.com/user-attachments/assets/820ede98-f3ed-43b2-981e-861ffbb39d9f)
![image](https://github.com/user-attachments/assets/69e539ee-3ace-460c-b2b2-3678d2833445)

##### Asi mismo se contempla que si el usuario quiere cambiar de contraseña este pueda hacerlo, esto se hace medeinte el uso de un nuevo dialog el cual haga la validación de contraseña anterior y activar una nueva contraseña.
![image](https://github.com/user-attachments/assets/74d73238-f38a-4fab-821d-d6d2c72d4c3a)
![image](https://github.com/user-attachments/assets/ade3d935-6966-4093-bdd0-15303f556825)

----------------------------------------------------------------------------------------
### * Agregar usuario
#### El boton de Agregar usuario direcciona a una pantalla en la cual se le piden los datos del nuevo usuario por tanto se ocupa 

![image](https://github.com/user-attachments/assets/91bbf0b7-e570-4229-9ed2-5f51569a3b94)
##### Una vez recolectado los daos estos se validan  se realiza el servicio HTTP de post sobre la tabla de usuarios.
![image](https://github.com/user-attachments/assets/e145428a-48eb-411f-9be7-89df10c136f4)

![image](https://github.com/user-attachments/assets/c820bf8c-ca4a-49c6-b7d4-b99ae991d947)

--------------------------------------------------------------------------------------
### * Agregar pelicula

#### El botón de Agregar peliculas  lo direccionara a una pantalla la cual tiene el contenido para recolectar los datos correspondientes a la pelicula en el codigo html se definio de la sigueinte manera. 
![image](https://github.com/user-attachments/assets/72b76501-27e9-43b0-b656-c7f62b0e0815)
#### Asi mismo para guardar los datos en la base de datos se requiere de hacer un método que valide los datos que se ingresaron y los guarde en la tabla de pelicula, por tanto en el typescript se hace un metodo el cual hace una peticion o un servicio HTTP el cual hace un post sobre peliculas, 

![image](https://github.com/user-attachments/assets/72ef2714-f3dc-425f-b081-5b78038a2e63)

![image](https://github.com/user-attachments/assets/bef6f3cc-89c6-420c-8a4f-377bf4fb4355)

------------------------------------------------------------------------------------------

### -> Pantalla principal 
![image](https://github.com/user-attachments/assets/74d6d1de-0586-4fa9-b45e-26b274948c70)

### En la pantalla principal se muestra una tabla la cual contiene los datos reelevantes sobre las peliculas, por tanto en cada registro se hace una consulta get sobre las peliculas almacenadas en la base. 
![image](https://github.com/user-attachments/assets/8315eb97-2764-4f39-a7e9-83f3de411b0c)
#### En cada uno de los registros se tiene un apartado el cual tiene 3 acciones en especifico

===========================================================================================

##### * Boton de ver información

##### Cuando se requiere de información sobre una pelicula al dar clic en la acción aparecera un dialog el cual  contendrá la ifnromaci+ón completa de la película en htmml se ve la sigueitne manera.
![image](https://github.com/user-attachments/assets/766c3941-ef10-465c-9426-294eb6b8b67d)
##### para esto se hace mediante el uso del servicio de obtención de usuario por medio de una ID
![image](https://github.com/user-attachments/assets/d18bd7a9-2e9d-4e67-b1fa-81a165b29387)

![image](https://github.com/user-attachments/assets/a4208af5-e17f-4e96-9c1c-4987bc024ac3)

============================================================================================
##### * Botón de Eliminar la película 
##### Para eliminar una pelicula al dar clic mostrará un dialog el cual moestrara el mensaje de eliminación.

![image](https://github.com/user-attachments/assets/67d3336f-76da-4780-99e8-d06663313fbc)

##### Para cuando ya se requiere de la eliminación de la pelicula se efectua el servicio de delete pelicula. 

![image](https://github.com/user-attachments/assets/2ca16f5f-705e-42a5-ab71-6a3b25e6f9ad)

![image](https://github.com/user-attachments/assets/4b8a1ffc-924a-4f41-ae7c-73d827ed26ff)

============================================================================================
##### * Botón de Modificar una película 

##### En el caso de modificar o editar una pelicula cuando se de clic en editar mostrará un html el cual contiene la información de la película y el usuario de clic en el boton de  aceptar o cancelar, siendo asi el html es de la siguiente manera. 

![image](https://github.com/user-attachments/assets/ad07a0e5-7a72-40e1-90d6-da1233b8ad75)

##### Para validar cuando se editen campos se realiza un método en el typescript el cual hace un servicio sobre la pelicula siendo que se muestre update sobre la tabla de peliculas.
![image](https://github.com/user-attachments/assets/c62f71c2-972d-48d6-a34d-89324c177f32)

![image](https://github.com/user-attachments/assets/c35aa2a4-0f1c-44cc-9ce6-204d6cbc3094)

============================================================================================
## Servicios
#### En el archivo de servicios se realizan los métodos que se mandaran a llamar cuando se requiera de hacer una solicitud.
#### Se realizaron tanto para usuarios como para películas.
### -> Para Usuarios

#### * GET USUARIO 
![image](https://github.com/user-attachments/assets/127d6886-2637-43af-9fc4-2f945bf788d5)
##### El método regresa un arreglo de usuarios, este por medio de una solicitud HTTP esto mediante el puerto que se asigno para listen y con ello el nombre de tabla con la cual se trabajará.

#### * UPDATE USUARIO
![image](https://github.com/user-attachments/assets/e821d4dc-27ba-4ca2-aab1-9dcdf4cbce44)
##### El método permite hacer una modificación sobre un objeto o elemento de la api de usuarios al cual a la consulta se pasa el ID  y este hace uso de PUT para modificar el dato. 

#### * POST USUARIO 
![image](https://github.com/user-attachments/assets/5d2a3f2a-977f-4b4f-9095-b4be1517b09b)
##### En este método se aplica el uso de POST el cual permite ingresar un elelemtno nuevo o un nuevo usuario, por tanto se le asigna a la api de usuarios y se le pasan los datos.

#### * DELETE USUARIO
![image](https://github.com/user-attachments/assets/8419707b-6884-4df5-a494-3835404de2ab)
##### Para la eliminación de un elemento o de un usuario en este caso se hace uso de delete al cual se le manda como dato un ID.

### -> Para Películas

#### * GET PELICULA
![image](https://github.com/user-attachments/assets/80cafe0f-8af5-47fe-a392-8aeee9aac46a)
##### El método se aplica para la recuperación del arreglo de las peliculas que estan en la api.

#### * GET PELÍCULA POR ID
![image](https://github.com/user-attachments/assets/994e81a1-e74b-4639-86ed-bc0d883e7700)
##### Obtiene la pelicula por la solicitud put en la api de películas.

#### * UPDATE PELÍCULA 
![image](https://github.com/user-attachments/assets/60df0fef-fe91-4749-b42a-f722d743418f)

##### El método aplica los cambios sobre un id en especifico sobre la api de peliculas.

#### * POST PELÍCULA 
![image](https://github.com/user-attachments/assets/4df5141e-f913-4c50-a237-59c368bb7f00)
##### Agrega una película a la api de peliculas, agrega todos los datos  de la película. 

#### * DELETE PELÍCULA
![image](https://github.com/user-attachments/assets/b7fdcf1a-e02a-4222-a339-51ce7949cc61)
##### Se elimina una pelicula del almacenamiento de la api de películas, este lo hace mediante la especificación de un id.

#### * BUSCAR PELÍCULAS
![image](https://github.com/user-attachments/assets/f911012a-803b-45c8-ac8e-33b9e7581549)
##### Se buscan peliculas por medio del nombre en la api, la cual se recibe como parámetro.


#### * PELICULAS PAGINADAS
![image](https://github.com/user-attachments/assets/3c759a1e-69a8-4948-aa2e-01a9c551b626)
##### Para mostrar elementos en una tabla, para tener un orden se muestra con una cantidad de elementos o peliculas y si hay mas elementos que mostrar estos se paginen, por lo cual este requiere hacer una consulta a la api en la que se reciban como parámetros la pagina y el tamaño.




