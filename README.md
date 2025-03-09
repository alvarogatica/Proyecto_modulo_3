# Proyecto_modulo_3

 ### LINK AL PROYECTO: proyectomod3.netlify.app

 ## INTRODUCCION AL PROYECTO
 ### Este proyecto consiste en una landing page de un proveedor de baterias. donde se muestra un poco de lo que consiste el instrumento como tambien sus productos mas relevantes ademas de un footer con informacion de contacto. Si bien es cierto, los botones de ruta no llevan a ningun lugar, es para tener una idea de lo que se puede hacer visualmente con un poco de html y css.

 ## OBJETIVOS DEL PROYECTO
 1. Crear una landing page simple
 2. El Landing Page debe utilizar HTML
 3. El Landing Page debe utilizar CSS
 4. Debe contar con Header, Main, "Area de productos", Footer
 5. Que sea Responsive en varios dispositivos con uno de MediaQuery (opcional)

## SOLUCION AL PROYECTO EN HTML/CSS

## Contamos con un archivo index.html, un archivo style.css y una carpeta con los assets que utlizamos, como imagenes en el proyecto.

### En la segmento inicial y toda la seccion header que se relaciona con la parte superior del Landing page

```HTML
<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Proyecto 3</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <nav class="navbar">
        <img src="/assets/logobat.avif" alt="" class="logo">
        <ul class="nav-links">
            <li class="active"><a href="#"></a>Inicio</li>
            <li><a href="#"></a>Acerca del Instrumento</li>
            <li><a href="#"></a>Productos</li>
            <li class="btn"><a href="#"></a>Contacto</li>
        </ul>
        <img src="/assets/menubutn.webp" alt="" class="menu-btn">
    </nav>
    <header>
        <div class="header-content">
            <h2>El mundo de la bateria</h2>
            <div class="line"></div>
                <h1>Tempo God</h1>
                <a href="#" class="btn">Mas informacion</a>
        </div>
    </header>
```

### En el siguiente segmento tenemos el "content" o "contenido" del Landing Page

```HTML
<main>
        <section class="about">
            <div class="about-content">
            <h1>Sobre el Instrumento</h1>
            <div class="line"></div>
            <p>Una batería es un conjunto de tambores, platillos y otros instrumentos de percusión, que se colocan en soportes para ser tocados por un solo músico,​ con baquetas en ambas manos y los pies accionando los pedales que controlan el platillo del hi-hat y el golpeador del bombo.</p>
            <a href="https://es.wikipedia.org/wiki/Bater%C3%ADa_(instrumento_musical)#:~:text=Una%20bater%C3%ADa%20es%20un%20conjunto,y%20el%20golpeador%20del%20bombo." class="btn">Mas info</a>
            </div>
        </section>
        <section class="products">
            <div class="title">
                <h1>Algunos Productos</h1>
                <div class="line"></div>
            </div>
            <div class="row">
                <div class="col">
                    <img src="/assets/yamaha.jpg" alt="Foto de Yamaha Drum">
                    <h4>Yamaha</h4>
                    <p>La marca de baterias YAMAHA es una de las maximas exponentes del mundo de la percusion</p>
                    <a href="https://usa.yamaha.com/products/musical_instruments/drums/index.html" class="btn">Mas Info</a>
                </div>
                <div class="col">
                    <img src="/assets/tama.webp" alt="Foto de Tama Drum">
                    <h4>Tama</h4>
                    <p>La marca de bateria Tama es una de las maximas exponentes del mundo de la percusion</p>
                    <a href="https://www.tama.com/asia/" class="btn">Mas Info</a>
                </div>
            </div>
        </section>
    </main>
```

### En el siguiente segmento tenemos el footer, donde se encuentra nuestra direccion y metodos de contacto junto a un mensaje de copyright clasico

```HTML
<footer>
        <section class="footer">
            <p>Club de Golf 7 Rios, Los Angeles, Bio Bio, Chile | Telefono: 973177098 | Email: alvaroandresgaticariquelme@gmail.com</p>
            <p>Copyright © 2025 Proyecto 3</p>
        </section>
    </footer>
```

### Finalizando los segmentos agregamos un pequeño script que nos ayuda a que nuestro menu y barra de navegacion sean responsivas

```HTML
<script>
        const menuBtn = document.querySelector('.menu-btn')
        const navlinks = document.querySelector('.nav-links')

        menuBtn.addEventListener('click', () => {
            navlinks.classList.toggle('mobile-menu');
        });
    </script>
</body>
</html>
```

### Solucion Completa del Archivo index.html

```HTML
<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Proyecto 3</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <nav class="navbar">
        <img src="/assets/logobat.avif" alt="" class="logo">
        <ul class="nav-links">
            <li class="active"><a href="#"></a>Inicio</li>
            <li><a href="#"></a>Acerca del Instrumento</li>
            <li><a href="#"></a>Productos</li>
            <li class="btn"><a href="#"></a>Contacto</li>
        </ul>
        <img src="/assets/menubutn.webp" alt="" class="menu-btn">
    </nav>
    <header>
        <div class="header-content">
            <h2>El mundo de la bateria</h2>
            <div class="line"></div>
                <h1>Tempo God</h1>
                <a href="#" class="btn">Mas informacion</a>
        </div>
    </header>
    <main>
        <section class="about">
            <div class="about-content">
            <h1>Sobre el Instrumento</h1>
            <div class="line"></div>
            <p>Una batería es un conjunto de tambores, platillos y otros instrumentos de percusión, que se colocan en soportes para ser tocados por un solo músico,​ con baquetas en ambas manos y los pies accionando los pedales que controlan el platillo del hi-hat y el golpeador del bombo.</p>
            <a href="https://es.wikipedia.org/wiki/Bater%C3%ADa_(instrumento_musical)#:~:text=Una%20bater%C3%ADa%20es%20un%20conjunto,y%20el%20golpeador%20del%20bombo." class="btn">Mas info</a>
            </div>
        </section>
        <section class="products">
            <div class="title">
                <h1>Algunos Productos</h1>
                <div class="line"></div>
            </div>
            <div class="row">
                <div class="col">
                    <img src="/assets/yamaha.jpg" alt="Foto de Yamaha Drum">
                    <h4>Yamaha</h4>
                    <p>La marca de baterias YAMAHA es una de las maximas exponentes del mundo de la percusion</p>
                    <a href="https://usa.yamaha.com/products/musical_instruments/drums/index.html" class="btn">Mas Info</a>
                </div>
                <div class="col">
                    <img src="/assets/tama.webp" alt="Foto de Tama Drum">
                    <h4>Tama</h4>
                    <p>La marca de bateria Tama es una de las maximas exponentes del mundo de la percusion</p>
                    <a href="https://www.tama.com/asia/" class="btn">Mas Info</a>
                </div>
            </div>
        </section>
    </main>
    <footer>
        <section class="footer">
            <p>Club de Golf 7 Rios, Los Angeles, Bio Bio, Chile | Telefono: 973177098 | Email: alvaroandresgaticariquelme@gmail.com</p>
            <p>Copyright © 2025 Proyecto 3</p>
        </section>
    </footer>
    <script>
        const menuBtn = document.querySelector('.menu-btn')
        const navlinks = document.querySelector('.nav-links')

        menuBtn.addEventListener('click', () => {
            navlinks.classList.toggle('mobile-menu');
        });
    </script>
</body>
</html>
```

### Ahora procedemos a mostrar el archivo de estilos style.css para mostrar como se fueron manejando los respectivos estilos, diferenciados en clases para que se pueda entender de mejor manera.

```CSS
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

a {
    text-decoration: none;
}

ul {
    list-style: none;
}

.active {
    color: #4e9df8;
    text-decoration: underline;
    font-weight: bold;
}

body , html {
    overflow-x: hidden;
}

.navbar {
    display: flex;
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    justify-content: space-between;
    padding: 20px;
    color: whitesmoke;
}
.navbar .logo {
    max-width: 100px;
    min-width: 100px;
}

.nav-links {
    display: flex;
    align-items: center;
}

.nav-links li {
    margin: 0 30px;
}

header {
    width: 100vw;
    height: 100vh;
    background-image: url(/assets/drumsheader1.jpg);
    background-position: bottom;
    background-size: cover;
    display: flex;
    align-items: flex-end;
    justify-content: center;
}

.header-content {
    margin-bottom: 150px;
    color: whitesmoke;
    text-align: center;
}

.header-content h2 {
    font-size: 4vmin;
}
 .line {
    width: 150px;
    height: 4px;
    background: #5099ec;
    margin: 10px auto;
    border-radius: 5px;
 }

 .header-content h1 {
    font-size: 7vmin;
    margin-top: 50px;
    margin-bottom: 30px;
 }

 .btn {
    padding: 8px 15px;
    background-color: #5099ec;
    border-radius: 30px;
    color: whitesmoke;
 }

.menu-btn {
    position: absolute;
    top: 30px;
    right: 30px;
    width: 40px;
    cursor: pointer;
    display: none;
}

section {
    width: 80%;
    margin: 80px auto;
}

.about {
    width: 100%;
    height: 100vh;
    background-image: url(/assets/drumbackabout.jpg);
    background-position: center;
    background-size: cover;
    background-repeat: no-repeat;
    display: flex;
    align-items: center;
}

.about-content {
    width: 50%;
    padding: 50px;
    color: whitesmoke;
    display: flex;
    align-items: center;
    flex-direction: column;
}

.about-content h1 {
    font-size: 7vmin;
}

.about-content .line {
    margin-bottom: 50px;
}
.about-content p {
    color: white;
}

.about-content .btn {
    margin-top: 40px;
}

.title {
    text-align: center;
    font-size: 4vmin;
    color: #5099ec;
}

.row {
    display: flex;
    align-items: center;
    width: 100%;
    justify-content: space-between;
}

.row .col {
    display: flex;
    flex-direction: column;
    align-items: center;
}

.row .col img {
    border-radius: 5%;
}

.products .row {
    margin-top: 50px;
}

h4 {
    font-size: 3vmin;
    color: #5099ec;
    margin: 20px auto;
}

p {
    color: #7c7c7c;
    padding: 0px 40px;
}

.products .btn {
    margin-top: 30px;
}

.footer {
    width: 100%;
    min-height: 100px;
    padding: 20px 80px;
    margin: 0;
    background: #484872;
    text-align: center;
}

.footer p {
    color: whitesmoke;
    margin: 20px auto;
}

 @media only screen and (max-width: 850px) {
    .menu-btn {
        display: block;
    }
    .navbar {
        padding: 0;
    }
    .logo {
        position: absolute;
        max-width: 100px;
        min-width: 100px;
        top: 30px;
        left: 30px;
    }
    .nav-links {
        flex-direction: column;
        width: 100%;
        height: 100vh;
        justify-content: center;
        background: #484872;
        margin-top: -2000px;
        transition: all 0.5s ease;
    }
    .mobile-menu {
        margin-top: 0px;
        border-bottom-right-radius: 30%;
    }
    .nav-links li {
        margin: 30px auto;
    }
    .about-content{
        width: 100%;
    }
    .row {
        flex-direction: column;
    }
    .row .col {
        margin: 20px auto;
    }
    .col img {
        max-width: 90%;
    }
    .footer {
        padding: 10px;
    }
 }

 img {
    transition: transform 0.3s ease;
 }

 img:hover {
    transform: scale(1.1);
 }
 .btn:hover {
    background: whitesmoke;
    color: #5099ec;
    box-shadow: 2px 2px 5px #00000056;
 }

 li:hover {
    color:#5099ec;
    cursor: pointer;
 }
```
### Cabe recordar que es solo como demostracion de lo que puede llegar a hacerse con un poco de html y css de manera responsiva
