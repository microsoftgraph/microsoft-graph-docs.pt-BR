---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 27225482ef5999a8808d0dcafeab9c80beea3b88
ms.sourcegitcommit: 7dc8ca82a8b2c25c5084e6b3121688766c9c14a6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/02/2021
ms.locfileid: "50072399"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Post post = new Post();
ItemBody body = new ItemBody();
body.contentType = BodyType.TEXT;
body.content = "content-value";
post.body = body;
post.receivedDateTime = CalendarSerializer.deserialize("2016-10-19T10:37:00Z");
post.hasAttachments = true;
Recipient from = new Recipient();
EmailAddress emailAddress = new EmailAddress();
emailAddress.name = "name-value";
emailAddress.address = "address-value";
from.emailAddress = emailAddress;
post.from = from;
Recipient sender = new Recipient();
EmailAddress emailAddress1 = new EmailAddress();
emailAddress1.name = "name-value";
emailAddress1.address = "address-value";
sender.emailAddress = emailAddress1;
post.sender = sender;
post.conversationThreadId = "conversationThreadId-value";
LinkedList<Recipient> newParticipantsList = new LinkedList<Recipient>();
Recipient newParticipants = new Recipient();
EmailAddress emailAddress2 = new EmailAddress();
emailAddress2.name = "name-value";
emailAddress2.address = "address-value";
newParticipants.emailAddress = emailAddress2;
newParticipantsList.add(newParticipants);
post.newParticipants = newParticipantsList;
post.conversationId = "conversationId-value";
post.createdDateTime = CalendarSerializer.deserialize("2016-10-19T10:37:00Z");
post.lastModifiedDateTime = CalendarSerializer.deserialize("2016-10-19T10:37:00Z");
post.changeKey = "changeKey-value";
LinkedList<String> categoriesList = new LinkedList<String>();
categoriesList.add("categories-value");
post.categories = categoriesList;
post.id = "id-value";
Post inReplyTo = new Post();
post.inReplyTo = inReplyTo;
LinkedList<Attachment> attachmentsList = new LinkedList<Attachment>();
FileAttachment attachments = new FileAttachment();
attachments.lastModifiedDateTime = CalendarSerializer.deserialize("2016-10-19T10:37:00Z");
attachments.name = "name-value";
attachments.contentType = "contentType-value";
attachments.size = 99;
attachments.isInline = true;
attachments.id = "id-value";
attachmentsList.add(attachments);
AttachmentCollectionResponse attachmentCollectionResponse = new AttachmentCollectionResponse();
attachmentCollectionResponse.value = attachmentsList;
AttachmentCollectionPage attachmentCollectionPage = new AttachmentCollectionPage(attachmentCollectionResponse, null);
post.attachments = attachmentCollectionPage;

graphClient.groups("{id}").threads("{id}").posts("{id}")
    .reply(post)
    .buildRequest()
    .post();

```