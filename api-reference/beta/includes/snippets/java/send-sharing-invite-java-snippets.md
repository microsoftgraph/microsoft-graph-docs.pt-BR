---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 545de9d7069b84b7a495582cb12601eb1ded5de5
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35861135"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<DriveRecipient> recipientsList = new LinkedList<DriveRecipient>();
DriveRecipient recipients = new DriveRecipient();
recipients.email = "ryan@contoso.org";

recipientsList.add(recipients);

String message = "Here's the file that we're collaborating on.";

boolean requireSignIn = True;

boolean sendInvitation = True;

LinkedList<String> rolesList = new LinkedList<String>();
rolesList.add("write");

String password = "password123";

int expirationDateTime = 7/15/2018 2:00:00 PM;

graphClient.me().drive().items("{item-id}")
    .invite(requireSignIn,rolesList,sendInvitation,message,recipientsList,expirationDateTime,password)
    .buildRequest()
    .post();

```