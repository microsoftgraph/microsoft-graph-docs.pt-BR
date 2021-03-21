---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fc9155787aeb4ca940ab0b372e718d40cb805994
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50960565"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var roleAssignments = await graphClient.RoleManagement.DeviceManagement.RoleAssignments
    .Request()
    .GetAsync();

```