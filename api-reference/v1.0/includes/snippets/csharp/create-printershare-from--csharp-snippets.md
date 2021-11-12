---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 303fc9b0d4d6e78d1538286a1011ade853935752fc2640237d246db4d16a9449
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57156869"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var printerShare = new PrinterShare
{
    DisplayName = "ShareName",
    AllowAllUsers = false,
    AdditionalData = new Dictionary<string, object>()
    {
        {"printer@odata.bind", "https://graph.microsoft.com/v1.0/print/printers/{printerId}"}
    }
};

await graphClient.Print.Shares
    .Request()
    .AddAsync(printerShare);

```