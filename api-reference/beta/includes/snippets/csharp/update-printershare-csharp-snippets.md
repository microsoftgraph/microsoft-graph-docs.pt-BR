---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 32df7683a63a55c0df246b4f2e7fece089e24400
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50802357"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var printerShare = new PrinterShare
{
    Name = "ShareName",
    AdditionalData = new Dictionary<string, object>()
    {
        {"printer@odata.bind", "https://graph.microsoft.com/beta/print/printers/{id}"}
    }
};

await graphClient.Print.Shares["{printerShare-id}"]
    .Request()
    .UpdateAsync(printerShare);

```