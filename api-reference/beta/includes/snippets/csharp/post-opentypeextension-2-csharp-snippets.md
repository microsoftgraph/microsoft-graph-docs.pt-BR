---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a19d4da41226d775189e54a1795d27d745512372
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/16/2019
ms.locfileid: "37544122"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var extension = new OpenTypeExtension
{
    ExtensionName = "Com.Contoso.Referral",
    CompanyName = "Wingtip Toys",
    DealValue = 500050,
    ExpirationDate = "2015-12-03T10:00:00Z"
};

await graphClient.Me.Messages["AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl==="].Extensions
    .Request()
    .AddAsync(extension);

```