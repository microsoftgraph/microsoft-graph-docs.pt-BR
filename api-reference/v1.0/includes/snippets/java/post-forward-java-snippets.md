---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6b929fc5a290193461fadb799d9f774e7e1fdcf2af504aa88f2548399450470b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57214309"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String comment = "comment-value";

LinkedList<Recipient> toRecipientsList = new LinkedList<Recipient>();
Recipient toRecipients = new Recipient();
EmailAddress emailAddress = new EmailAddress();
emailAddress.name = "name-value";
emailAddress.address = "address-value";
toRecipients.emailAddress = emailAddress;

toRecipientsList.add(toRecipients);

graphClient.groups("{id}").threads("{id}").posts("{id}")
    .forward(PostForwardParameterSet
        .newBuilder()
        .withComment(comment)
        .withToRecipients(toRecipientsList)
        .build())
    .buildRequest()
    .post();

```