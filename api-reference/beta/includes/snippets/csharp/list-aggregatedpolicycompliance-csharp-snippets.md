---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7ff361b6d422b2e6cf888c5545dcb1877b47ba3b
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/15/2021
ms.locfileid: "53441493"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var aggregatedPolicyCompliances = await graphClient.TenantRelationships.ManagedTenants.AggregatedPolicyCompliances
    .Request()
    .GetAsync();

```