---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 00e4b3b013fe783cc21125142f433064c69e7e62
ms.sourcegitcommit: 503c72036c376a30e08c29df8e7730a7afcab66e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/10/2021
ms.locfileid: "52871423"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var monthlyPrintUsageByUser = await graphClient.Print.Reports.MonthlyPrintUsageByUser
    .Request()
    .GetAsync();

```