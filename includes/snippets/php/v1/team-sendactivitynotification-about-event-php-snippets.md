---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

<?php

// THIS SNIPPET IS A PREVIEW VERSION OF THE SDK. NON-PRODUCTION USE ONLY
$graphServiceClient = new GraphServiceClient($tokenRequestContext, $scopes);

$requestBody = new SendActivityNotificationPostRequestBody();
$topic = new TeamworkActivityTopic();
$topic->setSource(new TeamworkActivityTopicSource('text'));
$topic->setValue('Weekly Virtual Social');
$topic->setWebUrl('Teams webUrl');
$requestBody->setTopic($topic);
$previewText = new ItemBody();
$previewText->setContent('It will be fun!');
$requestBody->setPreviewText($previewText);
$requestBody->setActivityType('eventCreated');
$recipient = new TeamMembersNotificationRecipient();
$recipient->setOdataType('microsoft.graph.teamMembersNotificationRecipient');
$recipient->setTeamId('7155e3c8-175e-4311-97ef-572edc3aa3db');
$requestBody->setRecipient($recipient);

$graphServiceClient->teams()->byTeamId('team-id')->sendActivityNotification()->post($requestBody)->wait();

```