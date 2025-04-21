# Ejercicios locos

1. ¿Qué comando usarías para crear un directorio?

- [ ] mkdir app
- [ ] ls
- [ ] app
- [ ] cd app

2. ¿Qué comando podés usar para juntar dos archivos de texto llamado animales y cosas y ordenarlos por orden alfabetico en otro archivo llamado salida?

- [ ] cat animales cosas > salida
- [ ] animales > cosas > salida
- [ ] cat animales cosas | sort > salida
- [ ] cat cosas animales > sort > salida

3. Para __________ un repo local a GitHub debemos ____________ usando usuario y _________.

**RTA:** Para *pushear* un repo local a GitHub debemos *autenticar* usando usuario y *token*.

4. ¿Cómo hacer para iniciar un repo local con un README.md vacío en la CLI y hacer el primer commit?

mkdir repo
cd repo
git init
touch README.md
git add .
git commit -m "primer commit"

5. Considere el siguiente código de HTML.
```html
<aside>
  <img src="" alt="" />
  <nav>
    <ul>
      <li>Cosas 1</li>
      <li>Cosas 2</li>
      <li>Cosas 3</li>
    </ul>
  </nav>
</aside>
```
Escribir una abreviación de Emmet para generar el código.

`aside>(img+nav>ul>li{Cosas $}*3)`

6. Usando CSS Grid dibujar la bandera de Suecia a partir del siguiente HTML y CSS.

```html
<body>
  <div class="blue"></div>
  <div class="yellow-h"></div>
  <div class="yellow-v"></div>
</body>
```

```css
body {
  margin: 0;
  height: 100vh;
  display: grid;
  grid-template: 1fr 50px 1fr / 150px 50px 1fr;
}
```

**RTA:**

```css
.yellow-h, .yellow-v {
  background: #ffcd00;
}

.yellow-v {
  grid-area: 1 / 2 / 4 / 3;
}

.yellow-h {
  grid-area: 2 / 1 / 3 / 4;
}

.blue {
  background: #006aa7;
  grid-area: 1 / 1 / 4 / 4;
}
```

7. Usando CSS estándar y Flexbox crear un tablero de ajedrez a partir del siguiente HTML

`div.board>((div.black+div.white)*4+(div.white+div.black)*4)*4`

**RTA:**

```css
.board {
  width: 400px;
  height: 400px; 
  display: flex;
  flex-wrap: wrap;
}

.black {
  background: black;
}

.white, .black {
  width: 50px;
  height: 50px;
}
```

8. ¿Cómo hacer que una lista no ordenada no se muestre con los puntos y aparezca en horizontal? Escribir una regla en CSS para eso.

```css
ul {
  list-style: none;
  display: flex;
}
```

9. ¿Cómo linkear una hoja de estilos externa en el `<head>`?

```html
<link rel="stylesheet" href="styles.css" />
```


