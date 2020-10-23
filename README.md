# comedor IONIC
app para el comedor

al final se queda como un programa en ionic para usar una base de datos firebase

pasos para crear app ionic con firebase:

1.- ionic start Note --blank -angular

2.- nos metemos dentro del directorio: cd Note

3.- isntalamos angular fire and firebase paquetes con los comandos:
npm install firebase @angular/fire

4.- Logea en tu firebase consola: 
https://console.firebase.google.com

5.- click en añadir proyecto. > metes el nombre del proyecto, aceptas los google analitics> default acount for firebase. <creando proyecto> 

6.- Firebase> settings (la rueda dentada), project settings > bajas y dale al boton de </> para añadir el codigo a tu proyecto> poen el nombre de la App en este caso Note. Y registrar la App. continuar > dentro del sript seleccionar la clase creada FirebaseConfig el var (declaracion de variables no hace falta) hasta  que se cierra el parentesis con ;. 

7.- eso se copia en src/environment.prod.ts
export const environment = {
  production: true,
  firebaseConfig : {
    apiKey: "AIzaSyBWFmtkqd6lXDC0qKSYwwf6JGxdHzAMUdM",
    authDomain: "noteapp-1cd5a.firebaseapp.com",
    databaseURL: "https://noteapp-1cd5a.firebaseio.com",
    projectId: "noteapp-1cd5a",
    storageBucket: "noteapp-1cd5a.appspot.com",
    messagingSenderId: "813508480870",
    appId: "1:813508480870:web:15e86201f5ceda4d7542a7",
    measurementId: "G-767CJMVRNT"
  }

};
asi quedaria.

8.- configurar app module> app.module.ts y ya todo el codigo.