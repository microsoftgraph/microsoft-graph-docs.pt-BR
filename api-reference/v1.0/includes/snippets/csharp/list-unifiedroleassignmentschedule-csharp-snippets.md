---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6816ececa885b90685627ff7f0e6e855f6fee572
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/05/2022
ms.locfileid: "65207184"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var roleAssignmentSchedules = await graphClient.RoleManagement.Directory.RoleAssignmentSchedules
    .Request()
    .GetAsync();

```