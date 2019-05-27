---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f7a49d4220d24220a0079187b5a4c274d3902a72
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34462208"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var shifts = await graphClient.Teams["{teamId}"].Schedule.Shifts
    .Request()
    .Filter("sharedShift/startDateTime ge 2019-03-11T00:00:00.000Z and sharedShift/endDateTime le 2019-03-18T00:00:00.000Z and draftShift/startDateTime ge 2019-03-11T00:00:00.000Z and draftShift/endDateTime le 2019-03-18T00:00:00.000Z")
    .GetAsync();

```