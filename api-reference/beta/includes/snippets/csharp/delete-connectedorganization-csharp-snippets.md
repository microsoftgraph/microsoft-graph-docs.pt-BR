---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 3276712aab40f748497ed310017a403da58babdd
ms.sourcegitcommit: 496410c1e256aa093eabf27f17e820d9ee91a293
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2020
ms.locfileid: "46566611"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.IdentityGovernance.EntitlementManagement.ConnectedOrganizations["{id}"]
    .Request()
    .DeleteAsync();

```