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
    <main id="context" class="container-center">
      <img class="logo" src="~/Images/imagotipo-fransun.png" alt="Logo" />
      <section class="login-box" style="margin-bottom:1rem">
        <article>
          <div style="padding: 2rem 3rem 1rem 3rem;">
            <form>
              <fieldset>
                <div class="form-control">
                  <label for="UserName" style="margin-bottom: 1rem;"><i class="fas fa-user mr-3"></i>Usuario</label>
                  <input id="UserName" name="UserName" type="text" required="required" />
                </div>
                <br />
                <div class="form-control">
                  <label for="Password" style="margin-bottom: 1rem;"><i class="fas fa-lock mr-3"></i>Contraseña</label>
                  <input id="Password" name="Password" type="password" required="required" />
                </div>
              </fieldset>
              <br />
              <div class="buttons-toolbar">
                <button class="link" type="submit"><i class="fas fa-sign-in-alt mr-3"></i>Entrar</button>
              </div>
            </form>
          </div>
        </article>
      </section>
      <section class="login-box" style="margin-bottom:0">
        <article>
          <div style="padding:1rem 3rem;">
            <a style="text-decoration:none; text-align:center;display:block" href="@Url.Action("Manual","Login")"><i class="fas fa-book"></i>&nbsp;&nbsp;Descarga el manual de usuario</a>
          </div>
        </article>
      </section>
    </main>
    
    <!-- Animación -->
    <footer class="fixed-bottom">
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
