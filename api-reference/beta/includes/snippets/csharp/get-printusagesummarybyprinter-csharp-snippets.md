---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fbec28f5f8f8cd4bdaec4ec14c5a3927d8a756ce
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50441452"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var printUsageByPrinter = await graphClient.Print.Reports.DailyPrintUsageSummariesByPrinter["{id}"]
    .Request()
    .GetAsync();

```