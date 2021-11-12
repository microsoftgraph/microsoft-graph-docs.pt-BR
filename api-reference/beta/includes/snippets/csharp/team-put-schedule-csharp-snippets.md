---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a0a08ed99bf577d4a5efac87fedf5ab55982de1c3ca5eb6b50b18c3d35d5199d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57099598"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var schedule = new Schedule
{
    Enabled = true,
    TimeZone = "America/Chicago"
};

await graphClient.Teams["{team-id}"].Schedule
    .Request()
    .PutAsync(schedule);

```