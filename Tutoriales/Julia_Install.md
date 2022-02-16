## Cómo instalar Juila o otros accesorios.

Aqui daremos las instrucciones para instalar Julia y otros accesorios.

### Instalando Julia:

La instalación de los binarios de Julia es bastante sencilla:
    
        Ir a la [página: ](https://julialang.org/downloads/)
        
Allí elija la instalación de acuerdo al sistema operativo de su computadora. Hoy en día casi todas las computadoras ya son de 64bits, 
pero por las dudas constate si no es de 32 bits, en tal caso use el apropiado.
        
        Siga las instrucciones de instalación de acuerdo a su sistema. 
        
En todos los sistemas, luego de la instalación, la ejecución les dará una ```Terminal``` donde estará ejecutando el REPL. 
Allí ya puede ejecutar comandos de Julia. 

### Trabajando con Julia

Hay varias maneras de trabajar a la hora de escribir programas de cierta complejidad:
    
**1.** **Editor de texto** Usualmente para trabajar con códigos un poquito complicados es mejor hacerlo usando un editor de texto apropiado. 
    Es decir un editor que comprenda la sintaxis de Julia y nos marque distintas partes del código, 
    incluso nos ayude con la documentación. Para linux recomendamos `kate` o `geany`. Para Windows recomendamos [geany](https://www.geany.org/download/nightly-builds/) o [notepad++](https://notepad-plus-plus.org/downloads/v7.9.3/)
    
**2. Usando notebooks** Una vez que hayan adquirido un poco de experiencia es recomendable usar notebooks. 
    Los notebooks se trabajan en el browser que está configurado como principal es su sistema. 
    Recomendamos usar ** Chrome**.
    Tienen la ventaja que los códigos se pueden ejecutar por partes (distintas celdas) y se pueden agregar comentarios usando 
    el código markdown, lo cual permite introducir fórmulas matemáticas de forma similar a LaTeX.
    
   Para Julia tenemos al menos 3 posibilidades: 
        
   a) `Ijulia`, (**recomendado**) es un notebook similar a Jupyter, pero nativo de Julia. Las instrucciones para su instalació
        instalación las pueden encontrar [aquí:](https://github.com/JuliaLang/IJulia.jl)
        
        
   b) `Jupyter`, es muy similar al anterior, pero su instalación es un poquito más compleja. Tiene la ventaja que allí 
        se pueden correr códigos en Python. Si ya lo tiene instalado entonces puede usar este directamente de acuerdo a lo 
        que indican [aquí](https://datatofish.com/add-julia-to-jupyter/) (para Windows). Para Linux usar **anaconda**.
        
   c) `Pluto`, es un nuevo tipo de notebook que es muy intersante y tiene varias ventajas sobre los otros. Pero estas ventajas también lo hacen complicado para personas con poca experiencia en la escritura de códigos. Por lo tanto **No lo recomendamos**. 
   De todos modos, las instrucciones para instalarlos están [aquí](https://github.com/fonsp/Pluto.jl)
   
 ## Instalando IJulia
 
 Para ello debe instalar el *paquete* con el código necesario. En la consola REPL ingrese el comando `]`eso le dará acceso al administrador de paquetes. Una ves allí escriba: (alternativamente, desde el REPL simplemente ingrese: Pkg.add("IJulia")).
 
    add Ijulia
    
A continuación (una vez instalado) salga del administrador de paquetes con el comando `borrar` o `delete` e ingrese:

    using IJulia
    notebook()
    
La primera vez que ejecute este comando tomará un tiempo apreciable hasta que se complete el cargado del sofware y se compile el código. En particular, la primera vez le preguntará si desea instalar **Jupyter**, si no lo tiene ya instalado acceda a ello. En tal caso instalará otro paquete, llamado `Conda.jl`. 
Una vez completado el proceso le debería aparecer una página en su browser donde podrá comenzar a trabajar con su notebook.
Cada vez que comienze a trabajar deberá llamar al REPL e ingresar los dós últimos comandos. 


       
