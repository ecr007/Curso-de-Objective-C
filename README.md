# Curso-de-Objective-C

# Primeros pasos con Objective-C
	- Que es Objective-C 02:23
	- Instalación de Objective-C 04:11
	- Hola Mundo con Objective-C 05:59

# La comunicación de Objective-C con el ordenador
	- Las funciones en Objective-C 05:45
	- Elementos de un programa en Objective-C 04:48

# Unidades para guardar información con Objective-C
	- Variables y constantes en Objective-C 05:16

		int x;
		x = 5;
		NSLog(@"El numero es: %i", x);

		// En Swift no es necesario el @

		Para definir constantes se usa la palabra reservada
		#define CONSTATE = VALOR;

	- Especificadores en Objective-C

		Son los tipos de datos que le especificaremos al lenguaje que debe pintar.

		int => %i
		float => %f
		char => %c
		char[n] => %s
		string => %@ || %s
		long => %ld
		long long => %lld
		double => %lf
		punteros => *

	- El puntero en Objective-C

		Un puntero es en palabras llanas el que que apunta la memoria de otra variable o objeto
		o lo que sea

		int VAR1 = 5;
		int * VAR2 = &VAR1;

		Para declarar un puntero se coloca * delante de la variable
		Para asignar la posición en memoria de una variable se coloca & delante de esta


	- Ejemplo de uso de puntero

		* scanf("especificador",direccion de memoria donde se guardara) -> Esta funcion lo que
		hace es guardar una entrada en la posicion de memoria de una variable

		NSLog(@"Con solo dos decimales %.2f",VarDouble) -> con ese .2 lo que hace es permitir esa
		cantidad de decimales solamente.

	- Operadores matemáticos en Objective-C

		OK, los de siempre

# Estructuras en Objective-C
	- Bloques o grupos de variables

	Son estructuras "Struct" que me permiten tener funcionalidades aisladas

	Struct cordenadas{
		float latitud;
		float longitud;
	};

	// Usar, instancion el struct
	Struct cordenadas instancia;

	instacia.latiud = 6.00;
	instancia.longitud = 30.0490394;

	// Tambien se puede usar typedef (Definicion de tipo)

	typedef Struct{
		float latitud;
		float longitud;
	} NAMESTRUCT;

	NameStruct ins;
	ins.latitud = 34.3434;
	ins.longitud = 34.45454656;


# Condicionales en Objective-C
	- Bifurcaciones y bucles en Objective-C

		Condiciones if if-elese switch
		Bucles while for do while

	- Estructuras de control: IF
		OK
	- Estructuras de control: SWITCH
		OK
	- Estructuras de control: FOR
		OK
	- Estructuras de control: WHILE y DO... WHILE
		OK

# Programación orientada a objetos en Objective-C
	- Conceptos de programación orientada a objetos

		Explicación de las clases

	- Explicación sobre la programación orientada a objetos

		Explicación de las clases, Mas conceptos

	- Objeto y clase en Objective-C

		Mas Explicación

	- Herencia con Objective-C 03:47

		Mas Explicación

	- Las Clases en Objective-C
		OK

	- Los métodos para cada clase 01:32
	- Los mensajes entre objetos 01:41
	- Tipos de datos en Objective-C 02:16

# Frameworks en Objective-C
	- Framework Foundation

	- Framework NSObject

		Es el objeto principal

	- Framework NSString

		Es la clase que se encarga de de gestionar las cadenas

		NSString * NomVar = @"Valor";

		El tamaño de un string lo obtengo de la siguiente manera:

		NSLog(@"Tamaño => %lu",(usigned long)NomVar.lenght);

		// Si te fijas el tamaño es un numero demacionado grande y no es un entero
		// Tambien se puede castear a un entero, pero por seguridad se hace con %lu y (usingned long)

	- Framework NSMutableString

		Esta clase se usa para interactuar aun mas con las cadenas, por ejemplo concatenar un valor

		NSMutableString * VarName = [[NSMutableString alloc] initWithString: @"Valor"];

		// Concatenamos
		[VarName appendString: @" Mas Texto OK !!"];

		El Mutable se le agrega a las clases para que estas puedan mutar.
		Ej: NSMutableArray

	- Framework NSArray

		Es la clase que me permite manejar arreglos en swift

		ej: NSArray * frutas = @[@"Mango", @"Piña", @"Melon"];

		Si quiero agregar un un array que se pueda gestionar lo mutamos

		Ej:

		NSMutableArray * frutasOK = [[NSMutableArray alloc] initWithObject: @"Mango", @"Piña", @"Melon"];

		// Agregamos informacion
		[frutasOK addObject: @"Cereza"];


# La aplicación móvil en Objective-C
	- Nuestra primera app con Xcode

	- Storyboard de nuestra app 02:47

# Patrón de diseño estructural con Objective-C
	- Patrón MVC o Modelo Vista Controlador 03:19
	- Patrón IBOulet 06:37
	- IBOulet por código 07:28
	- Patrón IBAction 07:49
	- Entender el patrón MVC 04:18

# Arquitectura en Software con Objective-C
	- Delegado en Objective-C 07:14
	- Protocolo en Objective-C 03:18

# Los errores con Xcode
	- Debugger en Objective-C 06:30

# Ejercicio práctico. App: WebServices
	- Storyboard de nuestra app 09:07
	- Array de datos de la app 09:20
	- TableView para la app WebServices 07:46
	- PopUp en nuestra app 08:07
	- Juego de preguntas: Vista Controlador 06:17
	- Modelo en el juego de preguntas 07:55
	- Implementación en la app de juego de preguntas 03:19
	- Despedida de Objective-C
