---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a5df72d9c67f1d25d83955eaa04691d78b18a79a
ms.sourcegitcommit: 972d83ea471d1e6167fa72a63ad0951095b60cb0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2022
ms.locfileid: "65247637"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var roleManagementPolicyAssignments = await graphClient.Policies.RoleManagementPolicyAssignments
    .Request()
    .Filter("scopeId eq '/' and scopeType eq 'Directory'")
    .GetAsync();

```