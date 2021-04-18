<html lang="en">
<head>
          <meta charset="UTF-8">
          <meta http-equiv="X-UA-Compatible" content="IE=edge">
          <meta name="viewport" content="width=device-width, initial-scale=1.0">
          <title>Adivina</title>
</head>
<body>
                    <A href="https://amilsandovalfrancisco.zyrosite.com/">Regresar al menu </A>     

          <script>
               var min = 1;
               var max = 100;
               var intentos = 0;
               var nombre = prompt('Bienvenido al juego adivina numero, ingresa tu nombre');
               var numero;
               var aleatorio = Math.floor(Math.random()* max - min + 1) + min;
              
               for(intentos; intentos < 10; intentos++ )
               {
                       numero =parseInt( prompt(nombre+' ingresa un numero entre el: '+min+ ' y el '+max));

                       if(numero >= min && numero <= max)
                       {
                              if(numero < aleatorio)
                              {
                                        alert('El numero que ingreso es menor');
                              }
                              else if(numero > aleatorio)
                              {
                                        alert('El numero que ingreso es mayor');
                              }
                              else if(numero = aleatorio)
                              {
                                  break;
                              }
                       }
                       else
                       {
                                 alert('Debes de ingresar un numero entre '+min+ 'y el '+max);
                       }

               }
               if(numero == aleatorio)
               {
                         alert('Felicidades, adivinaste el numero en '+(intentos+1)+' intentos');
               }
               else 
               {
                         alert('Agotaste el numero de intesto permitidos, suerte para la proxima !!!!');
               }
          </script>
</body>
</html> 
