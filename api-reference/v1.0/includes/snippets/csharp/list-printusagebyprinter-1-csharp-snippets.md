---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a160ccad2ecc153512b6f7e2a6d2bfc84169c74b329f65e244ebac08e777b8c2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57156359"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var dailyPrintUsageByPrinter = await graphClient.Reports.DailyPrintUsageByPrinter
    .Request()
    .GetAsync();

```