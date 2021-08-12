---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 28d20bda2bc5379919b2aabe5066880186cab4b8c491802b43be4cafb214f7e1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54275251"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var monthlyPrintUsageByPrinter = await graphClient.Print.Reports.MonthlyPrintUsageByPrinter
    .Request()
    .GetAsync();

```