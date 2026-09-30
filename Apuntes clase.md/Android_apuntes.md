# 📱 ANDROID — APUNTES DE CLASE

# 1 Primeros layouts XML
## 1.1 Los layouts
Los layauts son archivos contenedores que definen la estructura visual y la organización de los elementos en la pantalla de una aplicaión, su estructura es:
```xml
 <LinearLayout xmlns:android="http://schemas.android.com/apk/res/android"
        android:orientation="horizontal"
        android:gravity="center"
        android:layout_width="match_parent"
        android:layout_height="wrap_content">
```
Esta es la estructura principal, en ella podemos encontrar la orientacion del contenedor, la aliniación de el con gravity, el ancho del contenedor y el alto del contenedor. Si hacemos zoom al ancho y al alto vemos que tenemos match parent y wrap content. March parent manda la orden de que se ocupe todo elespacio posible del padre. En el otro lado de la moneda tenemos wrap content mandando la orden de ocupar el espacio maximo que el texto requiera.
El primer layout es el principal y es el contenedor que va a poseer la pantalla. Este va a marcar la colocaión de toodos los elementos, si la alineación es vertical todos lo elementos se van a colocar de forma vertical, si se alínea al centro todos van a ir centrados...
```xml
 </LinearLayout>
```
Como es lógico tenemos al final un cierre del contenedor. Este cierre se encuentra al final del contenido.

## Textview es un elemento de android que nos permite incluir texto. 

```xml 
<TextView
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:text="Iniciar Sesión"
        android:textSize="24sp"
        android:layout_marginTop="24dp"/>
```
Aqui podemos ver un elemento muy interesante 24sp y 24dp. Sp se utiliza generalmente para el tamaño de letra y depende de la configuración del tamaño de letra que tenga configurado el usuario.Dp depende de la densidad de pixeles que tiene la pantalla y se utiliza para distancias que queremos que queden "más fijas".
Ahora debemos de reocrdar los conceptos de marging y de padding. Marging es el espacio fuera del contenedor y padding es el espacio entre el contenido y el contenedor.
MARGIN
↓
┌───────────────────────────────┐
│                               │
│     PADDING                   │
│     ↓                         │
│     ┌───────────────────┐     │
│     │     CONTENIDO     │     │
│     └───────────────────┘     │
│                               │
└───────────────────────────────┘

## Edit text es un elemento de android que le permite al usuario introduccir texto 

```xml
<EditText
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:hint="Contraseña"
        android:inputType="textPassword"
        android:layout_marginTop="24dp"/>
```

Hint es la funcion que nos permite poner un texto sombreado que se quitara cuando el usuario escriba. Sirve para indicar a este que debe de poner ahí.

## Button
Button es un contenedor de android que nos permite introduccir un botón 
```xml
<Button
        android:id="@+id/button3"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:text="Entrar"
       />
```
text nos permite meter un texto dentro del botón