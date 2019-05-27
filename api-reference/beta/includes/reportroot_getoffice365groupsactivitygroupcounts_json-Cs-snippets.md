---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: bcedae9c632ef0d55e7bfcad469cb9273eba418c
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34441385"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getOffice365GroupsActivityGroupCounts = await graphClient.Reports.GetOffice365GroupsActivityGroupCounts('D7')
    .Request()
    .GetAsync();

```