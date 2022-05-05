---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 35f9adbe54ab02e5d1fb38759182768258c99f68
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/05/2022
ms.locfileid: "65205331"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var unifiedRoleAssignmentSchedule = await graphClient.RoleManagement.Directory.RoleAssignmentSchedules["{unifiedRoleAssignmentSchedule-id}"]
    .Request()
    .GetAsync();

```