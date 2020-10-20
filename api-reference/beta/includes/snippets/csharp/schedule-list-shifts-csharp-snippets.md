---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f7a49d4220d24220a0079187b5a4c274d3902a72
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/20/2020
ms.locfileid: "48612648"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var shifts = await graphClient.Teams["{teamId}"].Schedule.Shifts
    .Request()
    .Filter("sharedShift/startDateTime ge 2019-03-11T00:00:00.000Z and sharedShift/endDateTime le 2019-03-18T00:00:00.000Z and draftShift/startDateTime ge 2019-03-11T00:00:00.000Z and draftShift/endDateTime le 2019-03-18T00:00:00.000Z")
    .GetAsync();

```