---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: df2848d0e37a2e02406b8691033ea146e12de023
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/21/2021
ms.locfileid: "51921141"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var printerShare = new PrinterShare
{
    Name = "name-value",
    AdditionalData = new Dictionary<string, object>()
    {
        {"printer@odata.bind", "https://graph.microsoft.com/beta/print/printers/{id}"}
    }
};

await graphClient.Print.Shares
    .Request()
    .AddAsync(printerShare);

```