---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5ffa06c1317d5b364bdee2436d9937ed3487d670
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/15/2021
ms.locfileid: "53442679"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var unifiedRoleAssignmentScheduleInstance = await graphClient.RoleManagement.Directory.RoleAssignmentScheduleInstances["{unifiedRoleAssignmentScheduleInstance-id}"]
    .Request()
    .GetAsync();

```