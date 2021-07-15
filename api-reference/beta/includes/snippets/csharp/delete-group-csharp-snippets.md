---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8416fa7cd9334525e5bb2543d6e37c265f78737a
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/15/2021
ms.locfileid: "53445042"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Policies.MobileAppManagementPolicies["{mobilityManagementPolicy-id}"].IncludedGroups["{group-id}"].Reference
    .Request()
    .DeleteAsync();

```