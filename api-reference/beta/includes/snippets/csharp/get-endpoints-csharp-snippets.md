---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 63278b5707a5bfab87a605ad73c8892b7a40958d
ms.sourcegitcommit: 6ec748ef00d025ee216274a608291be3c1257777
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/27/2021
ms.locfileid: "50015497"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var reportRoot = await graphClient.Print.Reports["dailyPrintUsageSummariesByPrinter"]
    .Request()
    .GetAsync();

```