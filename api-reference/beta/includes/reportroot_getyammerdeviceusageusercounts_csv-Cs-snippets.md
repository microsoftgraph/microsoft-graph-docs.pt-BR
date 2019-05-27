---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c02c201b366e9d76a0c37239b411aaca2b9923af
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34482070"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getYammerDeviceUsageUserCounts = await graphClient.Reports.GetYammerDeviceUsageUserCounts('D7')
    .Request()
    .GetAsync();

```