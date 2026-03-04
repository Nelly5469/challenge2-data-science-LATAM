	columnas con yes y no
Churn			
customer.Partner		tiene_pareja
customer.Dependents		tiene_dependientes
phone.PhoneService		tiene_suscripcion_serv_tel * se va a reemplazar por 2 siguientes nuevas
phone.MultipleLines		tiene_mas_de_1_linea_tel
				tiene_1_linea_tel
(nueva)				tiene_serv_internet
internet.InternetService	es_internet_dsl ['DSL'=1 'Fiber optic'=0]	
internet.OnlineSecurity		tiene_seguridad_enlinea
internet.OnlineBackup		tiene_respaldo_enlinea	
internet.DeviceProtection	tiene_proteccion_dispositivo
internet.TechSupport 		tiene_soporte_tecnico_mayor
internet.StreamingTV		tiene_tv_cable
internet.StreamingMovies	tiene_stream_peliculas
account.PaperlessBilling	es_factura_enlinea



	trato especial
customer.gender			es_hombre	['Female'=0,Male'=1]
account.Contract		es_contrato_xanio
				es_contrato_mesxmes
				es_contrato_x2anios
	

	otras
customer.SeniorCitizen		es_mayoroigual_65_anios