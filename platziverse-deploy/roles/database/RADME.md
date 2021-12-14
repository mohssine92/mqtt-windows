scripts de automatizacion 
palybooks : contiene la informacion como yo voy a desplegar mi app , defino tareas como por ej cpy directori al servidor
            a la maquina virtual ocen , aws .. ejecute ese comando , lanze ese servicio etc ..
            tiene dependencias : roles . instalan redis , postgres como hemos instalado en nuestra maquina local
            lo mismo tenemos que hacer en maquina virtual ocen  .
            estos roles lo ofrece ansible dentro de otra plataforma sellama ansible glaxy

roles :  el que encarga de  instalar postgresql y redis ,y hacer la config inicial (roles descargados)
meta  :  definir que dependecias tiene nuestro rol - vamos a decir dependemos de rol postgresql y redis 
vars  :  donde sobre escribimos las variables del modulo de postgres
tasks :  va contener las tareas que voy a ejecutar

vars : sobre escribir variables que tiene postgresql el modulo de ansible de postgresql paraque se acomoda a nuestros necesidades 