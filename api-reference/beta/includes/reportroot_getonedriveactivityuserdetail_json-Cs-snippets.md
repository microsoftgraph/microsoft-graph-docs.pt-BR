---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7099cb67fbb20c402bbb90af8ce71b28bdbe8735
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34441147"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getOneDriveActivityUserDetail = await graphClient.Reports.GetOneDriveActivityUserDetail('D7')
    .Request()
    .GetAsync();

```