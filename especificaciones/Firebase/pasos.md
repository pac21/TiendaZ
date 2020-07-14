Una vez instalado el firebase en src/main.js agregamos

import firebase from 'firebase'

# Luego debemos crear la bd en la pagina de firebase

# Creamos un proyecto
Lo abrimnos y le damos que es para app web

# Le colocamos un apodo y registramos la aplicacion:
Nos dan el script para colocarlo en nuestro proyecto de Vue

## Creamos una nueva carpeta en src llamada firebase:
Adentro colocamos el script

## Despues debemos instanciarlo en src/main.js:
Colocamos:

let app = null
firebase.auth().onAuthStateChanged(() => {
	if(!app){
		new Vue({
			router,
			render: h => h(App)
		}).$mount('#app')
	}
})

# Nos vamos a ir a la consola:
En la parte izquieda en desarrollo precionamos authentication
para autentificar los datos que vamos a añadir como el login

# Apretamos configurar metodos de inicio de sesion:
Le damos en correo electronico/contraseña
Presionamos los dos botones de habilitar y guardamos

