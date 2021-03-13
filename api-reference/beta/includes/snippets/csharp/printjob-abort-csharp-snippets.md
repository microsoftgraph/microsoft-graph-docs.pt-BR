---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 528badfac444fbc8ee5f3ebb8da20c3bcf1a917d
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50795974"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Print.Printers["{printer-id}"].Jobs["{printJob-id}"]
    .Abort(null)
    .Request()
    .PostAsync();

```