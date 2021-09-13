---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5a113db0dc88bc7287eb3ace49ca9a90019fe40c9aedc62606e2c8ea162e592f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57102688"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var extension = new OpenTypeExtension
{
    ExtensionName = "Com.Contoso.Estimate",
    AdditionalData = new Dictionary<string, object>()
    {
        {"companyName", "Contoso"},
        {"expirationDate", "2016-07-30T11:00:00Z"},
        {"DealValue", "1010100"},
        {"topPicks", "[\"Employees only\",\"Add spouse or guest\",\"Add family\"]"}
    }
};

await graphClient.Groups["{group-id}"].Threads["{conversationThread-id}"].Posts["{post-id}"].Extensions["{extension-id}"]
    .Request()
    .UpdateAsync(extension);

```