# Usuarios y Contraeñas
# Admin: admin, contraseña: 123
# Usuario 1: jordan1, contraseña: pass1
# Usuario 2: isaac2, contraseña: pass2

    def iniciar_sesion():
    	intentos = 0
    	while intentos < 3:
        	usuario = input("Ingrese su Nombre de Usuario: ")
        	contraseña = input("Ingrese su Contraseña: ")
        
        	if (usuario == "admin" and contraseña == "123") or \
           	(usuario == "jordan1" and contraseña == "pass1") or \
           	(usuario == "isaac2" and contraseña == "pass2"):
            print("¡Bienvenido al Gestor de Notas UFidélitas!")
            return True
        else:
            print("Usuario o Contraseña incorrectos. Intente nuevamente.")
            intentos += 1
            
    print("Número máximo de intentos alcanzado. Saliendo del programa.")
    return False

    def menu_principal():
    	while True:
        	print("\n--- Menú ---")
        	print("1. Registro de estudiantes y materias")
        	print("2. Ingreso y validación de notas")
        	print("3. Consulta de calificaciones individuales")
        	print("4. Módulo de informes")
        	print("5. Salir")
        
        	opcion = input("Seleccione una opción: ")
        
        	if opcion == "1":
            	modulo_registro()
        	elif opcion == "2":
            	modulo_ingreso_notas()
        	elif opcion == "3":
            	modulo_consulta_calificaciones()
        	elif opcion == "4":
            	modulo_informes()
        	elif opcion == "5":
            	print("Gracias por Usar el Gestor de Notas. ¡Hasta luego!")
            	break
        	else:
            	print("Opción no Válida. Intente nuevamente.")

	def modulo_registro():
    	print("Módulo de Registro de Estudiantes y Materias")
    	# Registro de estudiantes y materias

	def modulo_ingreso_notas():
    	print("Módulo de Ingreso y Validación de Notas")
    	# Ingresar y validar notas

	def modulo_consulta_calificaciones():
    	print("Módulo de Consulta de Calificaciones Individuales")
    	# Consulta calificaciones

	def modulo_informes():
    	while True:
	        print("\n--- Módulo de Informes ---")
	        print("1. Promedio General por Materia")
	        print("2. Estudiante con Mejor Rendimiento")
	        print("3. Volver al Menú Principal")
        
	        opcion = input("Seleccione una Opción: ")
	        
	        if opcion == "1":
	            informe_promedio()
	        elif opcion == "2":
	            informe_mejor_rendimiento()
	        elif opcion == "3":
	            break
	        else:
	            print("Opción no Válida. Intente Nuevamente.")

	def informe_promedio():
	    print("Informe: Promedio general por materia")
	    # Calculadota del promedio y mostrar el promedio
	
	def informe_mejor_rendimiento():
	    print("Informe: Estudiante con mejor rendimiento")
	    # Mostrar el mejor rendimiento
	
	# Inicio del programa
	if __name__ == "__main__":
	    if iniciar_sesion():
	        menu_principal()
