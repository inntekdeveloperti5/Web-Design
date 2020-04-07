# Estructura del Navbar

![Navbar](https://raw.githubusercontent.com/inntekdeveloperti5/Web-Design/master/Document/Blob/Navbar.PNG "Navbar")

```html
<body>
  <header>
  
    <nav class="navbar navbar-expand-lg navbar-light bg-g-blue mb-5 shadow-6dp">
      <div class="container">
      
        <!-- Titulo del portal -->
        <a class="navbar-brand text-white" href="#">
          <span class="filter-shadow"><i class="fas fa-globe mr-3"></i></span>
          <span class="text-shadow">Nombre del portal</span>
        </a>
        
        <!-- Boton para colapsar menu, solo visible en pantallas pequeñas -->
        <button class="navbar-toggler text-white" type="button" data-toggle="collapse" data-target="#navbarportal" aria-controls="navbarportal" aria-expanded="false">
          <i class="fas fa-bars"></i>
        </button>
        
        <!-- Area de menus -->
        <div class="collapse navbar-collapse" id="navbarportal">
          <hr />
          
          <ul class="navbar-nav mr-3">
            <li class="nav-item dropdown">
              <a class="nav-link text-white dropdown-toggle" href="#" id="catalogosmenu" role="button" data-toggle="dropdown" aria-haspopup="true" aria-expanded="false">
                <span class="filter-shadow"><i class="fas fa-user-book mr-2"></i></span>
                <span class="text-shadow">Catalogos</span>
              </a>
              <div class="dropdown-menu shadow" aria-labelledby="catalogosmenu">
                <a class="dropdown-item text-muted" href="#">Link</a>
              </div>
            </li>
          </ul>
          
          <ul class="navbar-nav">
            <li class="nav-item dropdown">
              <a class="nav-link text-white dropdown-toggle" href="#" id="usermenu" role="button" data-toggle="dropdown" aria-haspopup="true" aria-expanded="false">
                <span class="filter-shadow"><i class="fas fa-user-circle mr-2"></i></span>
                <span class="text-shadow">Usuario</span>
              </a>
              <div class="dropdown-menu shadow" aria-labelledby="usermenu">
                <a class="dropdown-item text-muted" href="#">
                  <i class="fas fa-sign-out-alt mr-3"></i>Cerrar Sesión
                </a>
              </div>
            </li>
          </ul>
        
        </div>
        
      </div>
    </nav>
  </header>
  <!-- CODE -->
</body>
```

## Backgroud color
```css
.bg-g-blue {
    background: rgb(0,123,255);
    background: linear-gradient(0deg, rgb(0,102,211) 0%, rgb(0,123,255) 100%);
    border-top: 1px solid rgb(0,123,255);
    border-bottom: 1px solid rgb(0,102,211);
}
```

## Icon Shadow
```css
.filter-shadow {
    filter: drop-shadow(0 0 3px rgba(0,0,0,0.3)) drop-shadow(0 0 1px rgba(0,0,0,0.2));
}
```

## Text Shadow
```css
.text-shadow {
    text-shadow: 0 0 3px rgba(0,0,0,0.3), 0 0 1px rgba(0,0,0,0.2);
}
```

