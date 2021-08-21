---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4b1aea48e870de0c78081a50e11d1fd183909c2707382d3d85b864048e579c0c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56899712"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var unifiedRoleManagementPolicyAssignment = await graphClient.Policies.RoleManagementPolicyAssignments["{unifiedRoleManagementPolicyAssignment-id}"]
    .Request()
    .GetAsync();

```