---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: cabfde47d95071917c30e03557d25075e28ac99f
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35476736"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var notifyTeam = true;

var startDateTime = 10/8/2018 12:00:00 AM;

var endDateTime = 10/15/2018 12:00:00 AM;

await graphClient.Teams["{teamId}"].Schedule
    .Share(notifyTeam,startDateTime,endDateTime)
    .Request()
    .PostAsync();

```