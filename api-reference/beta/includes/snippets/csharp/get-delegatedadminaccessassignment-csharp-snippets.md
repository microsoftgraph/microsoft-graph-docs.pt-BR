---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 438b20beca8e1955337168cb2342837222ca2b14
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/05/2022
ms.locfileid: "65202404"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var delegatedAdminAccessAssignment = await graphClient.TenantRelationships.DelegatedAdminRelationships["{delegatedAdminRelationship-id}"].AccessAssignments["{delegatedAdminAccessAssignment-id}"]
    .Request()
    .GetAsync();

```