---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 04640234310079bd23af69209292dad557d69ea4
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35878342"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var extension = new Extension
{
    AdditionalData = new Dictionary<string, object>()
    {
        {"@odata.type","microsoft.graph.openTypeExtension"}
    },
    ExtensionName = "Com.Contoso.Deal",
    CompanyName = "Alpine Skis",
    DealValue = 1010100,
    ExpirationDate = "2015-07-03T13:04:00Z"
};

await graphClient.Groups["f5480dfd-7d77-4d0b-ba2e-3391953cc74a"].Events["AAMkADVl17IsAAA="].Extensions
    .Request()
    .AddAsync(extension);

```