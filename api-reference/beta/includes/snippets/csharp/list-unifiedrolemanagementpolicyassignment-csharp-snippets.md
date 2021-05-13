---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e4a1da4b7e1b74124e6c275d739b568dc37ee1d2
ms.sourcegitcommit: b8b0e88b3ba9a434dc45f5ab640cb46f66fae299
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/13/2021
ms.locfileid: "52474321"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var roleManagementPolicyAssignments = await graphClient.Policies.RoleManagementPolicyAssignments
    .Request()
    .GetAsync();

```