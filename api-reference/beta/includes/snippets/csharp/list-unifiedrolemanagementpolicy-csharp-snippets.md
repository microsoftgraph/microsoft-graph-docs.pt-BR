---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 40ed7ba1ea539e5ad003206a6348eaad813bd56ad8ca048571a4bc537887e774
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57158231"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var roleManagementPolicies = await graphClient.Policies.RoleManagementPolicies
    .Request()
    .GetAsync();

```