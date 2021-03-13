---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e3bf1745a625af33c7e98dc50d56ae2efe14d0d9
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50774409"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var printUsageByUser = await graphClient.Reports.DailyPrintUsageByUser["{printUsageByUser-id}"]
    .Request()
    .GetAsync();

```