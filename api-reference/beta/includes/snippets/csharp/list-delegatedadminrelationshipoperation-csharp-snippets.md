---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2770a13abd3b8de1d37d856d3da2b55ed9f6ebbb
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/05/2022
ms.locfileid: "65207678"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var operations = await graphClient.TenantRelationships.DelegatedAdminRelationships["{delegatedAdminRelationship-id}"].Operations
    .Request()
    .GetAsync();

```