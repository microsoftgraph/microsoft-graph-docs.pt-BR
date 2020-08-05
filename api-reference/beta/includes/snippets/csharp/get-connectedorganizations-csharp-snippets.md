---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a11c450ef139462392328150bdcd78f2bcac4515
ms.sourcegitcommit: 496410c1e256aa093eabf27f17e820d9ee91a293
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2020
ms.locfileid: "46566556"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var connectedOrganizations = await graphClient.IdentityGovernance.EntitlementManagement.ConnectedOrganizations
    .Request()
    .GetAsync();

```