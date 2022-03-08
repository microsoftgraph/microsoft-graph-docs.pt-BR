---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 71c5f90eb7e90e8720f22c59920627a0bcdf0335
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2022
ms.locfileid: "63351076"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var unifiedRoleAssignment = await graphClient.RoleManagement.Directory.RoleAssignments["{unifiedRoleAssignment-id}"]
    .Request()
    .Expand("roleDefinition,principal,directoryScope")
    .GetAsync();

```