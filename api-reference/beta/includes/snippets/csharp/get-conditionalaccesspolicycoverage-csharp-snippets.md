---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a6c43f2101cd58c8019042d384ef980d1d94bb9e
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/15/2021
ms.locfileid: "53440117"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var conditionalAccessPolicyCoverage = await graphClient.TenantRelationships.ManagedTenants.ConditionalAccessPolicyCoverages["{managedTenants.conditionalAccessPolicyCoverage-id}"]
    .Request()
    .GetAsync();

```