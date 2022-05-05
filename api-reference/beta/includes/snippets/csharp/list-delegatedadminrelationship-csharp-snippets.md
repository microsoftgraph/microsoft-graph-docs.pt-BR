---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d64cad164e2d55ab32af481b89e5c0f68e1235a7
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/05/2022
ms.locfileid: "65210883"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var delegatedAdminRelationships = await graphClient.TenantRelationships.DelegatedAdminRelationships
    .Request()
    .GetAsync();

```