---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 04fdb23fa2f471b6dfae2a6dea73324414034c0dd937bf26a3dfbf079540663c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57327936"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var roleEligibilityScheduleInstances = await graphClient.RoleManagement.Directory.RoleEligibilityScheduleInstances
    .Request()
    .GetAsync();

```