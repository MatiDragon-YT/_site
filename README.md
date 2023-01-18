
<!DOCTYPE html>
<html lang="es">
<head>
	<title>Página Principal</title>
	<meta charset="utf-8">
	<meta http-equiv="X-UA-Compatible" content="IE=edge">
	<meta name="viewport" content="width=device-width, initial-scale=1">
	<link rel="stylesheet" type="text/css" href="./css/main.css">
  <meta name="description" content="Comienza a codificar SCM y JS con mayor fácilidad">
</head>
<body>

[h1][Bienvenido!]\
[h2 light][Comienza a codificar SCM y JS\ncon mayor fácilidad]

:::d-flex wrap mx-2
:::col-12 col-md-6 light c f-center h5 p-2
[mw-50 d-inline-block][Usando un bonito resaltador de sintaxis, junto a una amplia lista de comandos unicos y una documentacion en español :smile:]
:::center mx-4
[descargar](mods/c.md 'button')
:::
:::
:::col-12 col-md-6
```h5 h-50#one
```
:::
:::

:::col-12
##### Direcciones
[Discord](https://discord.gg/d5dZSfgBZr)
[GitHub](https://github.com/MatiDragon-YT)
[YouTube](https://youtube.com/@MatiDragon)
[Twitter](https://twitter.com/@MatiDragon)
:::
<script src="./js/main.min.js"></script>

<script>
const txt = [
`{$CLEO}
nop
const
	Pressed = Key.Pressed(VK.Oem3)
end
while true
	wait 0
	if Pressed
	then
		0@ = Actor.Create(PedType.Civil, #FAM1, 0.0, 0.0, 0.0)
		repeat wait 0
		until Pressed
		Actor.Release(0@)
	end
end`
]

let i = 0;
function typeWriter(x) {
  if (i < txt[x].length) {
    $('#one').innerText += txt[x][i++]
    setTimeout(typeWriter, Math.floor(Math.random() * 86), x)
  	hightlight.sb3($('#one'))
  }
}

typeWriter(0)
</script>
<style>
#one {
    z-index: -2;
    position: fixed;
    filter: blur(7px) opacity(16%);
    left: -2%;
    height: 150%;
    width: 120%;
    top: 6rem;
    overflow: hidden;
}
.d-inline-block {
	text-shadow: 0px 0px 3px #0a0d11;
}
pre {background: #0d1117;font-size: calc(1em + 2.5vh)!important;}
@media (min-width:768px) {
#one {
    z-index: 0;
    position: initial;
    filter: none;
    left: auto;
    height: 50vh;
		max-height: 28.65rem;
    width: auto;
    top: auto;
    overflow: auto;
}
.d-inline-block {
	text-shadow: none;
}
pre{background: #161b22;font-size: 1.25rem!important;}}
</style>
