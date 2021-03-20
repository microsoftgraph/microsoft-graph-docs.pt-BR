---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 31b9e150c4f13654814f27c66e651fa51980f765
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50953061"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var dailyPrintUsageSummariesByUser = await graphClient.Print.Reports.DailyPrintUsageSummariesByUser
    .Request()
    .GetAsync();

```