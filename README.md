# credit_assignment

Requiere del servicio: /credit/search_user

POST: /credit-assignment
	- Requiere de un token (Autoenthication Beaer token)
	- Antes de ejecutar el servicio valida que tenga cceso.
  - Json: {“investment”: 3000}
  - Archivo de configuracion configDB.json, configHttp.json y configMsSarchUsr.json


Responde en caso de exito 200 y json:
 {
   “credit_type_300”: 2, 
   “credit_type_500”: 2, 
   “credit_type_700”: 2}
}
 
Responde en caso de error:
 {
   "code": "credit_assignment_microservice",
   "message": "Mensaje a detalle",
   "status_code": 400
 }
