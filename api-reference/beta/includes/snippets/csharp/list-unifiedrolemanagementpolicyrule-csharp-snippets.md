---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 068722586ade22f5c368e552c6209175e9502197
ms.sourcegitcommit: b8b0e88b3ba9a434dc45f5ab640cb46f66fae299
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/13/2021
ms.locfileid: "52474285"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var effectiveRules = await graphClient.Policies.RoleManagementPolicies["{unifiedRoleManagementPolicy-id}"].EffectiveRules
    .Request()
    .GetAsync();

```