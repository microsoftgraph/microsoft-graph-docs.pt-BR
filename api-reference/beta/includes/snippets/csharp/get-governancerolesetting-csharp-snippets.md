---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ac2a701d48f291a1ed635f10955b13cb6c8651bc6a37f9d03cc38ea2c5b0c759
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56899780"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var governanceRoleSetting = await graphClient.PrivilegedAccess["{privilegedAccess-id}"].RoleSettings["{governanceRoleSetting-id}"]
    .Request()
    .GetAsync();

```