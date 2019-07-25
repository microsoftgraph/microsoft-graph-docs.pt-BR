---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c4fadabb3b5c9bd95bef6475abad4cbdbbd27018
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35716599"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var emailAddresses = new List<String>()
{
    "danas@contoso.onmicrosoft.com",
    "fannyd@contoso.onmicrosoft.com"
};

var mailTipsOptions = MailTipsType.AutomaticReplies | MailTipsType.MailboxFullStatus;

await graphClient.Me
    .GetMailTips(emailAddresses,mailTipsOptions)
    .Request()
    .PostAsync();

```