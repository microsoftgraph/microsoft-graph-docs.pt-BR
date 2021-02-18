---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4c9d17e1931bcfe80229c5ca8fe641d2009ba139
ms.sourcegitcommit: 42fdb068616222eb6b0813e93b33e830fc7eedc0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/17/2021
ms.locfileid: "50274917"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var shift = await graphClient.Teams["{teamId}"].Schedule.Shifts["{shiftId}"]
    .Request()
    .GetAsync();

```