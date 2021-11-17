---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 22d3dd4eb9e7f4392d7fecaf646b668afb8355b8b4d7466227904f81679f4e2d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57275252"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var conditionalAccessPolicyCoverage = await graphClient.TenantRelationships.ManagedTenants.ConditionalAccessPolicyCoverages["{managedTenants.conditionalAccessPolicyCoverage-id}"]
    .Request()
    .GetAsync();

```