---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5274fe0cd95babdb2907ce5ae087161e37d6b260
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34464374"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getSkypeForBusinessDeviceUsageUserCounts = await graphClient.Reports.GetSkypeForBusinessDeviceUsageUserCounts('D7')
    .Request()
    .GetAsync();

```