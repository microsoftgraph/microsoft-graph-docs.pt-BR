---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 78cbb0584a756cbb00ba2fa0cf09877a4efdc800021794396a85febb14c1ed42
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57273100"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var timeOffReason = new TimeOffReason
{
    DisplayName = "Vacation",
    IconType = TimeOffReasonIconType.Plane,
    IsActive = true
};

await graphClient.Teams["{team-id}"].Schedule.TimeOffReasons
    .Request()
    .AddAsync(timeOffReason);

```