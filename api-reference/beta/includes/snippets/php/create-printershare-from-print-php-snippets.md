---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

<?php

// THIS SNIPPET IS A PREVIEW VERSION OF THE SDK. NON-PRODUCTION USE ONLY
$graphServiceClient = new GraphServiceClient($tokenRequestContext, $scopes);

$requestBody = new PrinterShare();
$requestBody->setName('name-value');
$additionalData = [
	'printer@odata.bind' => 'https://graph.microsoft.com/beta/print/printers/{id}',
];
$requestBody->setAdditionalData($additionalData);

$result = $graphServiceClient->print()->shares()->post($requestBody)->wait();

```