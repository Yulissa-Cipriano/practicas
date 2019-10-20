#include <stdio.h>
main()
{
	int id=4; // int
	int nom_hosp=100; // char(100)
	int direccion=100; //char(100)
	int servicio=1; //boolean true=publico false=privado
	int no_trabajadores=3; // mediumInt
	int especialidad=30; // char(30)
	int horario=20; // char(20)
	int pacientes=3; // mediumInt
	int no_camas=3; // mediumInt
	int no_salas=2; // smallInt
	int no_elevadores=2; // smallInt
	int no_edificios=2; // smallInt
	int extension=4; // float
	int telefono=15; // char(15)
	int correo=30; // char(30)
	int pagina=50; // char(50)
	int nom_director=30; // char(30)
	int ranking=4; // int
	int fecha_apertura=3; // date aaaa-mm-dd
	
	//Calcular el tamaño de una fila
	int tam_fila;
	tam_fila=id+nom_hosp+direccion+servicio+no_trabajadores+especialidad+horario+pacientes+no_camas+no_salas+no_elevadores+no_edificios+extension+telefono+correo+pagina+nom_director+ranking+fecha_apertura;
	
	//Calcular el tamaño de una página
	int fil_por_pag=35;
	int tam_pag;
	tam_pag=tam_fila*fil_por_pag;
	
	//Calcular número de páginas
	long int num_registros=50627392;
	long int num_paginas;
	num_paginas=num_registros/fil_por_pag;
	
	printf("El tamaño de una fila en bytes es: %d",tam_fila);
	printf("\nEl tamaño de una pagina en bytes es: %d",tam_pag);
	printf("\nNumero de paginas: %d",num_paginas);
	printf("\nEl tamaño de la base de datos en bytes es: %d * %d = 20554708160",num_paginas,tam_pag);
}"# Tama-oBD" 
