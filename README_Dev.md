[checkmark]: https://raw.githubusercontent.com/mozgbrasil/mozgbrasil.github.io/master/assets/images/logos/logo_32_32.png "MOZG"
![valid XHTML][checkmark]

# Mozg\Itau

# Filiação Teste

	<codigo_empresa>J0026376210001060000011110</codigo_empresa>
	<chave_criptografia>S8G9F8C2E3R4K2FD</chave_criptografia>

# Database

SELECT * FROM `sales_flat_order` ORDER BY `entity_id` DESC LIMIT 1;

SELECT * FROM `sales_flat_order_payment` ORDER BY `entity_id` DESC LIMIT 1;

SELECT * FROM `mozg_api_debug` ORDER BY `debug_id` DESC LIMIT 1;

SELECT * FROM `mozg_event_data` ORDER BY `event_id` DESC LIMIT 1;

SELECT * FROM `mozg_event_data_queue`;

SELECT * FROM `mozg_order_payment` ORDER BY `entity_id` DESC LIMIT 1;



#


----
## Recorrencia

Para  o processo para recorrencia devendo informar o mesmo PaymentId

1 - Finalizar o pedido

2 - Pegar o pspReference e informar em PaymentId

http://127.0.0.1/public_html/magento-1.9.3.0-dev32/mozg_itau/process/notification/PaymentId/b6f727e7-2f19-422b-84a8-d0230b431dde/

No uso de RECURRING_CONTRACT 

Acesse em app/code/local/Mozg/Itau/Model/Api.php

Altere em recurringDetailReference sendo o PaymentId

Execute o Queue

Verá no historico do pedido "Criado o contrato de faturamento "
-----




## Contribuintes

Equipe Mozg

:cat2:
