---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: bcc4e3753e65b5f6071033bf199531180164ddc6
ms.sourcegitcommit: 503c72036c376a30e08c29df8e7730a7afcab66e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/10/2021
ms.locfileid: "52869930"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var unifiedRoleAssignmentMultiple = new UnifiedRoleAssignmentMultiple
{
    DisplayName = "NewName",
    Description = "A new roleAssignment"
};

await graphClient.RoleManagement.CloudPC.RoleAssignments["{unifiedRoleAssignmentMultiple-id}"]
    .Request()
    .UpdateAsync(unifiedRoleAssignmentMultiple);

```