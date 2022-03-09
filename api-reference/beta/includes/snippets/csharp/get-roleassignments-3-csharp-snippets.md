---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e5b4e00870a9e0b13e5b551c4cc93f0bb1e3ff8d
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/09/2022
ms.locfileid: "63396536"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var roleAssignments = await graphClient.RoleManagement.EntitlementManagement.RoleAssignments
    .Request()
    .Filter("appScopeId eq '/AccessPackageCatalog/4cee616b-fdf9-4890-9d10-955e0ccb12bc'")
    .Expand("principal")
    .GetAsync();

```