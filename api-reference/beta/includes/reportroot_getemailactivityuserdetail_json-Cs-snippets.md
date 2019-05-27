---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d75ea17788c38a44b37139ede0a6363e0115e093
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34442302"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getEmailActivityUserDetail = await graphClient.Reports.GetEmailActivityUserDetail('D7')
    .Request()
    .GetAsync();

```