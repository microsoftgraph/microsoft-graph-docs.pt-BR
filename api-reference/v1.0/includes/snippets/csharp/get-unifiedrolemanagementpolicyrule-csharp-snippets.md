---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d0f07aa83f55b50b3784c25d6d5d49030971b964
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/05/2022
ms.locfileid: "65204458"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var unifiedRoleManagementPolicyRule = await graphClient.Policies.RoleManagementPolicies["{unifiedRoleManagementPolicy-id}"].Rules["{unifiedRoleManagementPolicyRule-id}"]
    .Request()
    .GetAsync();

```