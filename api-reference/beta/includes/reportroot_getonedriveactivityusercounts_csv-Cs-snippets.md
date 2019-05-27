---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 0277ad0b4d98e12104de08784b5daccf42c74c86
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34441217"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getOneDriveActivityUserCounts = await graphClient.Reports.GetOneDriveActivityUserCounts('D7')
    .Request()
    .GetAsync();

```