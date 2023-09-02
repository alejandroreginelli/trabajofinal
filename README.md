
Algoritmo cajaRegitradoraSuperMercado
	Definir cp,p,tp,tf,td,cd,vu,cl,in,op Como Entero
	tf<-0
	td<-0
	cl<-232923
	in<-0
	   Mientras (in==0) Hacer
		   Escribir "===MENU==="
		   Escribir "1.VENDER"
		   Escribir "2.VER EL TOLTAL DEL DIA Y FINALIZAR"
		   Leer op
		   Segun op Hacer
			   1:
				   Limpiar Pantalla
				   Escribir "Ingrese la cantidad de productos a vender"
				   Leer cp
				   Para i<- 1 Hasta cp Con Paso 1 Hacer
					   Escribir "ingrese el valor del producto:",i
					   Leer p
					   Escribir "ingrese la cantidad de productos a vender:",i
					   Leer vp
					   tp<-p*vp
					   tf<-tf+tp
				   Fin Para
				   Escribir "INGRESE CLAVE DE LA CAJA REGISTRADORA"
				   Leer cl
				   si(cl==232923) Entonces
					   Escribir "INGRESE CANTIDAD DE DINERO ENTREGADA POR EL CLIENTE:"
					   Leer cd
					   vu<-cd-tf
					   Escribir "** Resumen de la compra**"
					   Escribir "El total de compra fue :$",tf
					   Escribir "El dinero entregado por el cliente :$",cd
					   Escribir "Vuelto del cliente $",vu
					   td<-td+tf
					   tf<-0
				   SiNo
					   Escribir "La clave es incorrecta"
					   
				   FinSi
			   2:
				   Limpiar Pantalla
				   in<-1
				   Escribir "Total de ventas del dia :$",td
			   De Otro Modo:
				   Escribir  "ingreso una opcion invalida"
				   
		   Fin Segun
	   Fin Mientras

	
FinAlgoritmo
