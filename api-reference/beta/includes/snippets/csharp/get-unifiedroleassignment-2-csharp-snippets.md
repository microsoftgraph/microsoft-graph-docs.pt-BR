---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fd110358f288a20e67b09ab4b62ad43d42d4e8c0
ms.sourcegitcommit: 0d6d39dd6450e0c5fd6844cb78aead00a0782e46
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2022
ms.locfileid: "63759236"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var unifiedRoleAssignment = await graphClient.RoleManagement.Directory.RoleAssignments["{unifiedRoleAssignment-id}"]
    .Request()
    .Expand("roleDefinition")
    .GetAsync();

```