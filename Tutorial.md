# jCorona - Workshop

[https://github.com/fjrdomingues/flag_jquery/blob/master/Tutorial.md](https://github.com/fjrdomingues/flag_jquery/blob/master/Tutorial.md)

Vamos construir uma página usando jQuery

# Instalação
O jQuery pode ser instalado de várias formas. O método mais indicado depende do projecto em que estamos a trabalhar. As opções mais comuns são:
 - Fazer **download** do ficheiro e importar localmente
 - Instalar usando **npm**, Yarn ou Bower
 - Usar um **CDN** (vamos usar este)

Dentro destas opções podem optar pela versão compressed/minified ou uncompressed. **Devemos usar sempre a minified.**

## Setup index.html
- Criar um ficheiro index.html
- Criar as tags básicas de html (html, head, body, style)
- Importar jQuery usando um CDN
- Adicionar title, header, h1 e #container

# Selectors

Selectors em jQuery permitem seleccionar elementos do DOM 
Usam a mesma sintaxe que CSS.

[w3schools - jQuery Selectors](https://www.w3schools.com/jquery/jquery_ref_selectors.asp)

## Adicionar estilo

Vamos adicionar algumas regras de estilo à página:

```css
body {
	margin: 0;
	font-family: 'Roboto', sans-serif;
	background: #f7f7f7;
	text-align: center;
}
header {
	color: black;
	text-align: center;
	background: white;
	box-shadow: 0px 9px 20px 0px rgba(0, 0, 0, 0.16);
	margin: 5px 8px;
}
header h1 {
	padding: 20px;
	margin: 0;
}
#container {
	margin-top: 50px;
	padding: 0 20%;
}
```

## jQuery Selectors

Antes da primeira função de jQuery vamos só adicionar o seguinte:

 - h2 com id="intro"
 - p com id="introPara" e span
 - h2 com class="titulo2"
 - p com id="para2" e span

### Selectors básicos

Com jQuery fica muito mais fácil selecionar elementos específicos de uma página

- Exemplo com h2, id, class e span
- Guardar objectos em variáveis

### Selectors mais avançados

Podemos também selecionar elementos pela ordem em que aparecem.

``` html
<table>  
	<tr>  
		<th>País</th>  
		<th>Casos</th>  
		<th>Recuperados</th>  
	</tr> 	 
	<tr>  
		<td>China</td>  
		<td>80849</td>  
		<td>66000</td>  
	</tr>  
	<tr>  
		<td>Portugal</td>  
		<td>245</td>  
		<td>2</td>  
	</tr>  
</table>
```

``` css
thead {
	background: white;
}
table, th, td {
	border: 1px solid grey;
	padding: 10px;
	text-align: left;
}
table {
	border-collapse: collapse;
	margin: 0 auto;
}
```

Exemplos com:
(put script on head)
- :first
- :last
- :even
- nth-child
- by [attr]=value
- all
- hide and show with button
- [https://www.w3schools.com/jquery/trysel.asp](https://www.w3schools.com/jquery/trysel.asp)

# Events

Events são funções que correm quando algo acontece na página. Pode ser um clique num botão, um hover com o rato, o momento em que página carregou todo o conteúdo, etc. A lista completa está em:
[https://api.jquery.com/category/events/](https://api.jquery.com/category/events/)

## Exemplos

- Click -> alert
- $(document).ready(function)
- mouseenter e mouseleave
- focus and blur
- keyup and e.target.value on an input
- change on select