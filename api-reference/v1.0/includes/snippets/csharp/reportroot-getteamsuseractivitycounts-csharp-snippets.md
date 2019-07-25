---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5ed21239791461ca20f96aaaf02a633226254b4f
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35855587"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports
    .GetTeamsUserActivityCounts('D7')
    .Request()
    .GetAsync();

```