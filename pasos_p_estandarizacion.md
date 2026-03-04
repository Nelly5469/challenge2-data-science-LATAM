	columnas con yes y no
Churn						churn
customer.Partner			tiene_pareja
customer.Dependents			tiene_dependientes
internet.OnlineSecurity		tiene_seguridad_enlinea
internet.OnlineBackup		tiene_respaldo_enlinea	
internet.DeviceProtection	tiene_proteccion_dispositivo
internet.TechSupport 		tiene_soporte_tecnico_mayor
internet.StreamingTV		tiene_tv_cable
internet.StreamingMovies	tiene_stream_peliculas
account.PaperlessBilling	es_factura_enlinea


	trato especial
customer.gender			es_hombre	['Female'=0,Male'=1]
internet.InternetService	es_internet_dsl ['DSL'=1 'Fiber optic'=0]
account.Contract		es_contrato_xanio
						es_contrato_mesxmes
						es_contrato_x2anios
account.PaymentMethod	es_pago_automatico ['Mailed check' 'Electronic check' = 0 'Credit card (automatic)' 'Bank transfer (automatic)' = 1]
						es_pago_por_correo
						es_pago_electronico
						es_pago_tarj_cred
						es_pago_transf_bancaria
phone.PhoneService			tiene_suscripcion_serv_tel * se va a reemplazar por 2 nuevas tiene_mas_de_1_linea_tel y tiene_1_linea_tel
phone.MultipleLines		tiene_mas_de_1_linea_tel
						tiene_1_linea_tel
(nueva)					tiene_serv_internet verificar que todas las columnas referentes coincidan en cantidad de clientes con servicio de internet
	

	otras
customer.SeniorCitizen		es_mayoroigual_65_anios
account.Charges.Monthly		total_serv_mes
account.Charges.Total 		total_gastado
Cuentas_Diarias				total_serv_mes_x_dia