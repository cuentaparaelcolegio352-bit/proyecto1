<!DOCTYPE html>
<html>
<head>
	<meta charset="utf-8">
	<meta name="viewport" content="width=device-width, initial-scale=1">
	<title>Login</title>
	<style>
			*{
					padding: 0px;
					margin: 0px;
					box-sizing: border-box;
					font-family: century gotic, sans-serif;
					text-align: center;
			}
			body{
				background-image: url(https://static.motor.es/fotos-noticias/2020/03/que-coche-es-rayo-mcqueen-202066150-1585635516_1.jpg);
				width: 100%;
				height: 100vh;
				background-size: cover;
				color: white;
			}
			form{
				background-color: rgba(56, 27, 27, 0.65);
				padding: 50px 20px;
				width: 90%;
				max-width: 400px;
				margin: 20vh auto;
				border-radius: 8px;
				box-shadow: 0 4px 10px rgba(0, 0, 0, 0.3);
			}
			h1, h2 {
				color: rgb(206, 203, 203);
				font-family: Kristen ITC;
			}
				input{
					width: 100%;
					padding: 9px;
					margin-top: 12px;
					font-size: 16px;
					border-radius: 5px;
				}
				input[type=´submit´]{
					background-color: #48e;
					color: #fff;
					width: 50%;
					margin: 22px auto;
					border: none;
					cursor: pointer;
					border-radius: 7px;
					box-shadow: 0 4px 10px rgba(0, 0, 0, 0.3);
				}
				input[type=´submit´]:hover{
					background-color: #369;
				}
				label{
					font-family: Berlin Sans FB Demi;
					font-size: 16px;
					margin-top: 18px;
				}
	</style>
</head>
<body>
	<div class="container">
		<form id="loginForm">
			<h1>Pagina de acceso</h1>
			<h2>David Miranda</h2>
			<br>
			<div class="mb-3">
				<label for="email">Usuario</label>
				<input type="email" class="form-control" id="email" required placeholder="ingrese Usaurario">
			</div>
			<div class="mb-3">
				<label for="password">contraseña</label>
				<input type="password" class="form-control" id="password" required placeholder="ingrese password">
			</div>
			<input type="submit" name="ingresar" value="ingresar">
		</form>
		<div id="menssage"></div>
	</div>
	<script>
		document.getElemetByid("LoginForm").eddEventListener("submit" ,function(event){
			event.preventDefault();

			var email = document.getElemetByid("email").value;
 	    var password = document.getElemetByid("password").value;
 	
 			if (email"eber@email.com" && password==="123"){
		    window.location.href="https://es.wikipedia.org/wiki/Wikipedia:Portada";
  }
  if (email"david@email.com" && password==="123"){
		    window.location.href="https://es.wikipedia.org/wiki/Wikipedia:Portada";
  }   	 
  else{
        document.getElemetByid("message").innerhtml"acceso denegado"

  }

	});
	</script>
</body>
</html>
