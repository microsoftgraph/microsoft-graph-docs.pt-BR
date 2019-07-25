---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fe0c565bd270539f86a9bf8903c22e8d3ac58542
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35873017"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getOneDriveUsageAccountCounts = await graphClient.Reports
    .GetOneDriveUsageAccountCounts('D7')
    .Request()
    .GetAsync();

```