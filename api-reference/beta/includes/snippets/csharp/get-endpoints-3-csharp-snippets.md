---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ee78ac01de0a4fb772c67120e39d9adbf7d679af
ms.sourcegitcommit: 503c72036c376a30e08c29df8e7730a7afcab66e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/10/2021
ms.locfileid: "52871395"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var dailyPrintUsageByPrinter = await graphClient.Print.Reports.DailyPrintUsageByPrinter
    .Request()
    .GetAsync();

```