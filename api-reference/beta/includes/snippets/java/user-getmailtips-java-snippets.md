---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e142bc0a353d7abcbbd327cf42a0a5a2497942a53dafa052a6e759b39176f08b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57275586"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<String> emailAddressesList = new LinkedList<String>();
emailAddressesList.add("danas@contoso.onmicrosoft.com");
emailAddressesList.add("fannyd@contoso.onmicrosoft.com");

EnumSet<MailTipsType> mailTipsOptions = EnumSet.of(MailTipsType.AUTOMATIC_REPLIES,MailTipsType.MAILBOX_FULL_STATUS);

graphClient.me()
    .getMailTips(UserGetMailTipsParameterSet
        .newBuilder()
        .withEmailAddresses(emailAddressesList)
        .withMailTipsOptions(mailTipsOptions)
        .build())
    .buildRequest()
    .post();

```