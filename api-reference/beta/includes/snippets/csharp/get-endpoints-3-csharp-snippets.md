---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e1ee423c6474b8459494e12275a3a3c9e2c9d27c
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50953172"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var dailyPrintUsageSummariesByPrinter = await graphClient.Print.Reports.DailyPrintUsageSummariesByPrinter
    .Request()
    .GetAsync();

```