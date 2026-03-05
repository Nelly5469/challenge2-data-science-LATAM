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

RENOMBRE DE COLUMNAS TRANSFORMADAS
Churn                                                 bool	CHURN
customer.gender                                       bool	ES_HOMBRE
customer.SeniorCitizen                                bool 	TIENE_PAREJA
customer.Partner                                      bool	TIENE_PAREJA
customer.Dependents                                   bool 	TIENE_DEPENDIENTES
customer.tenure                                      int64	NUM_MESES_CONTRATO
internet.OnlineSecurity                               bool	TIENE_SEGURIDAD_ENLINEA
internet.OnlineBackup                                 bool 	TIENE_RESPALDO_ENLINEA
internet.DeviceProtection                             bool	TIENE_PROTECCION_DISPOSITIVO
internet.TechSupport                                  bool	TIENE_SOPORTE_TECNICO_MAYOR
internet.StreamingTV                                  bool	TIENE_TV_CABLE
internet.StreamingMovies                              bool	TIENE_STREAM_PELIS
account.PaperlessBilling                              bool	ES_FACTURA_ENLINEA
account.Charges.Monthly                            float64	TOTAL_SERV_MES_DOLARES
account.Charges.Total                              float64	TOTAL_GASTADO_DOLARES
Cuentas_Diarias                                    float64	TOTAL_SERV_MESXDIA_DOLARES
account.Contract_MONTH-TO-MONTH                       bool	ES_CONTRATO_XMES
account.Contract_ONE YEAR                             bool	ES_CONTRATO_XANIO
account.Contract_TWO YEAR                             bool	ES_CONTRATO_X2ANIOS
account.PaymentMethod_BANK TRANSFER (AUTOMATIC)       bool	ES_PAGO_TRANSF_BANCARIA
account.PaymentMethod_CREDIT CARD (AUTOMATIC)         bool	ES_PAGO_TARJ_CRED
account.PaymentMethod_ELECTRONIC CHECK                bool	ES_PAGO_ELECTRONICO
account.PaymentMethod_MAILED CHECK                    bool	ES_PAGO_POR_CORREO
es_pago_automatico                                    bool	ES_PAGO_AUTOMATICO
phone__NO                                             bool	TIENE_1_LIN_TEL
phone__YES                                            bool	TIENE_MASDE_1_LIN_TEL
tiene_serv_internet                                   bool	TIENE_SERV_INTERNET

cols eliminadas
	phone__NO PHONE SERVICE                               bool	