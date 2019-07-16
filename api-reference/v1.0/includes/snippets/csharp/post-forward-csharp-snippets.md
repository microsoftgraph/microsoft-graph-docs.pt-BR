---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5103864baa63537e03f3d85431cf9b1740563c12
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/16/2019
ms.locfileid: "35739657"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var comment = "comment-value";

var toRecipients = new List<Recipient>()
{
    new Recipient
    {
        EmailAddress = new EmailAddress
        {
            Name = "name-value",
            Address = "address-value"
        }
    }
};

await graphClient.Groups["{id}"].Threads["{id}"].Posts["{id}"]
    .Forward(comment,toRecipients)
    .Request()
    .PostAsync();

```