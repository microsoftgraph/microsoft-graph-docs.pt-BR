---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 580ab999ffb72a22f7b0291aa984948bbd17bd20
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50803162"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var destinationPrinterId = "9a3b3956-ce5b-4d06-a605-5b0bd3e9ddea";

await graphClient.Print.Printers["{printer-id}"].Jobs["{printJob-id}"]
    .Redirect(destinationPrinterId,null)
    .Request()
    .PostAsync();

```