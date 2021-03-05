---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e1ee423c6474b8459494e12275a3a3c9e2c9d27c
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50465341"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var dailyPrintUsageSummariesByPrinter = await graphClient.Print.Reports.DailyPrintUsageSummariesByPrinter
    .Request()
    .GetAsync();

```