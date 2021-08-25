---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: eec48b9ead65f7c7492a280691ad64d843534ef0
ms.sourcegitcommit: 9b8abc940a68dac6ee5da105ca29800cb59775f6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/25/2021
ms.locfileid: "58513761"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var filterByCurrentUser = await graphClient.RoleManagement.Directory.RoleAssignmentScheduleRequests
    .FilterByCurrentUser(RoleAssignmentScheduleRequestFilterByCurrentUserOptions.Principal)
    .Request()
    .GetAsync();

```