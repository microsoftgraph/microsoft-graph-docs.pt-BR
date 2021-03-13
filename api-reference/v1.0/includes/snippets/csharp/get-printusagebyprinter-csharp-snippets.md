---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e1e2056e511ab6f24ed108cb8e62af5b21ddf262
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50774444"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var printUsageByPrinter = await graphClient.Reports.DailyPrintUsageByPrinter["{printUsageByPrinter-id}"]
    .Request()
    .GetAsync();

```