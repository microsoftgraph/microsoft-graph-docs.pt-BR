---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 3635545a18d9fdbad6fde5879af0ee0aeaee7033
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48964302"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Post post = new Post();
ItemBody body = new ItemBody();
body.contentType = BodyType.TEXT;
body.content = "I attached an event.";
post.body = body;
LinkedList<Attachment> attachmentsList = new LinkedList<Attachment>();
ItemAttachment attachments = new ItemAttachment();
attachments.name = "Holiday event";
Event item = new Event();
item.subject = "Discuss gifts for children";
ItemBody body1 = new ItemBody();
body1.contentType = BodyType.HTML;
body1.content = "Let's look for funding!";
item.body = body1;
DateTimeTimeZone start = new DateTimeTimeZone();
start.dateTime = "2019-12-02T18:00:00";
start.timeZone = "Pacific Standard Time";
item.start = start;
DateTimeTimeZone end = new DateTimeTimeZone();
end.dateTime = "2019-12-02T19:00:00";
end.timeZone = "Pacific Standard Time";
item.end = end;
attachments.item = item;
attachmentsList.add(attachments);
AttachmentCollectionResponse attachmentCollectionResponse = new AttachmentCollectionResponse();
attachmentCollectionResponse.value = attachmentsList;
AttachmentCollectionPage attachmentCollectionPage = new AttachmentCollectionPage(attachmentCollectionResponse, null);
post.attachments = attachmentCollectionPage;

graphClient.groups("1848753d-185d-4c08-a4e4-6ee40521d115").threads("AAQkADJUdfolA==")
    .reply(post)
    .buildRequest()
    .post();

```