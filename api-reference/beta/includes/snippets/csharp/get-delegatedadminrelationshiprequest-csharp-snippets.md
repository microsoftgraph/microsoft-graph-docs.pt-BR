---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a7598e5121c0ade0e19b5ddae9cbab82188fb761
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/05/2022
ms.locfileid: "65209141"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var delegatedAdminRelationshipRequest = await graphClient.TenantRelationships.DelegatedAdminRelationships["{delegatedAdminRelationship-id}"].Requests["{delegatedAdminRelationshipRequest-id}"]
    .Request()
    .GetAsync();

```