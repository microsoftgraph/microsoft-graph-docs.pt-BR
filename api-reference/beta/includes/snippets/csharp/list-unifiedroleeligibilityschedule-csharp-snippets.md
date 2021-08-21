---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fa696f22877f9fb349bb7ea68ae07685aab5bba2e10e1e7cf8dcaf7d2843daa8
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57101468"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var roleEligibilitySchedules = await graphClient.RoleManagement.Directory.RoleEligibilitySchedules
    .Request()
    .GetAsync();

```