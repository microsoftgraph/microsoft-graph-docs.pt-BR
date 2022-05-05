---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ddd5ac493ec51f8899aff7883320f8fb1fa80fc3
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/05/2022
ms.locfileid: "65203503"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var requests = await graphClient.TenantRelationships.DelegatedAdminRelationships["{delegatedAdminRelationship-id}"].Requests
    .Request()
    .GetAsync();

```