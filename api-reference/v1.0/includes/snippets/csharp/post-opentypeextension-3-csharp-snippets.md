---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 70a740c36c74229efdf854d8d3fc6948df0fa1ac
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50470852"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var extension = new OpenTypeExtension
{
    ExtensionName = "Com.Contoso.Deal",
    AdditionalData = new Dictionary<string, object>()
    {
        {"companyName", "Alpine Skis"},
        {"dealValue", "1010100"},
        {"expirationDate", "2015-07-03T13:04:00Z"}
    }
};

await graphClient.Groups["f5480dfd-7d77-4d0b-ba2e-3391953cc74a"].Events["AAMkADVl17IsAAA="].Extensions
    .Request()
    .AddAsync(extension);

```