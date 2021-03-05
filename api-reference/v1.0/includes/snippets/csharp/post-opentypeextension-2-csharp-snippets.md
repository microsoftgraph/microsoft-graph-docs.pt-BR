---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5786deec5c0576c83e6f07f16e3b56bb8ea54efe
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50470855"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var extension = new OpenTypeExtension
{
    ExtensionName = "Com.Contoso.Referral",
    AdditionalData = new Dictionary<string, object>()
    {
        {"companyName", "Wingtip Toys"},
        {"dealValue", "500050"},
        {"expirationDate", "2015-12-03T10:00:00Z"}
    }
};

await graphClient.Me.Messages["AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl==="].Extensions
    .Request()
    .AddAsync(extension);

```