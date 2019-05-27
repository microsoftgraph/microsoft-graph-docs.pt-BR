---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 11deed0714b5c0bdc5728ebc0e5d4bf461073c68
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34434910"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var report = await graphClient.Reports.GetTeamsDeviceUsageUserCounts('D7')
    .Request()
    .GetAsync();

```