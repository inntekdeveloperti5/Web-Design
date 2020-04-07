# Estructura del Login

![Login](https://raw.githubusercontent.com/inntekdeveloperti5/Web-Design/master/Document/Blob/Login.PNG "Login")

```html
<!DOCTYPE html>
<html lang="es-MX">
  <head>
    <meta name="viewport" content="width=device-width, initial-scale=1, shrink-to-fit=no" />
    <meta http-equiv="Content-Type" content="text/html; charset=utf-8" />
    <meta name="distribution" content="global" />
    <meta name="author" content="G.F. Inntek" />
    <meta charset="utf-8" />
    <title>Título del portal</title>
    <!-- Agregar Likns CSS Bootstrap -->
    <!-- Agregar Likns CSS Portal -->
  </head>
  <body class="bg-light">
    <main id="context" class="position-absolute d-flex flex-column justify-content-center align-items-center h-100 w-100">
      <img class="mb-4" src="~/Images/imagotipo-fransun.png" style="height:130px;filter:drop-shadow(0 0 7px #f8f9fa);" />
      <div class="bg-white rounded shadow-6dp pt-5 pb-4 pl-5 pr-5" style="max-width:500px;width:100%">
        <form>
          <div class="form-group">
            <label class="text-muted" for="exampleInputEmail1">Email Address</label>
            <input type="email" class="form-control text-center" id="exampleInputEmail1" required="required" />
          </div>
          <div class="form-group">
            <label class="text-muted" for="exampleInputPassword1">Password</label>
            <input type="password" class="form-control text-center" id="exampleInputPassword1" required="required" />
          </div>
          <div class="form-group form-check pl-1">
            <div class="custom-control custom-checkbox">
              <input type="checkbox" class="custom-control-input" id="customControlAutosizing" />
              <label class="custom-control-label text-muted" for="customControlAutosizing">Recordar usuario</label>
            </div>
          </div>
          <div class="text-right">
            <button type="submit" class="btn btn-link text-decoration-none">
            <span><i class="fas fa-sign-in-alt mr-2"></i>Iniciar Sesión</span>
            </button>
          </div>
        </form>
      </div>
    </main>
    <footer class="fixed-bottom" style="z-index:-1;">
      <svg class="editorial" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink"
        viewBox="0 24 150 28" preserveAspectRatio="none">
        <defs>
          <path id="gentle-wave" d="M-160 44c30 0 58-18 88-18s 58 18 88 18 58-18 88-18 58 18 88 18 v44h-352z" />
        </defs>
        <g class="parallax">
          <use xlink:href="#gentle-wave" x="50" y="0" fill="#9eb5d9" />
          <use xlink:href="#gentle-wave" x="50" y="3" fill="#b6c7e2" />
          <use xlink:href="#gentle-wave" x="50" y="7" fill="#cedaec" />
        </g>
      </svg>
    </footer>
    <!-- Agregar Likns Scripts FontAwesome + Solid || Regular -->
    <!-- Agregar Likns Scripts Knockout -->
    <!-- Agregar Likns Scripts JQuery -->
    <!-- Agregar Likns Scripts Bootstrap Bundle -->
    <!-- Agregar Likns Scripts Repository -->
    <!-- Agregar Likns Scripts Portal -->
  </body>
</html>
```

## CSS del logo

```css
img.logo {
    height: 130px;
    margin-bottom: 1.5rem;
}
```

## CSS de la animacion

```css
.parallax > use {
    animation: move-forever 12s linear infinite;
}

    .parallax > use:nth-child(1) {
        animation-delay: -5s;
    }

    .parallax > use:nth-child(2) {
        animation-delay: -7s;
        animation-duration: 15s
    }

    .parallax > use:nth-child(3) {
        animation-delay: -9s;
        animation-duration: 20s
    }

@keyframes move-forever {
    0% {
        transform: translate(-90px, 0%)
    }

    100% {
        transform: translate(85px, 0%)
    }
}

.editorial {
    display: block;
    width: 100%;
    height: 10em;
    max-height: 100vh;
    margin: 0;
}
```
