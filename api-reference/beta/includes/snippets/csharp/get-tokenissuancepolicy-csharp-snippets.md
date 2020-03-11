---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c30c4ecc76b3c233d214b1ab3957bb8950d6c3aa
ms.sourcegitcommit: c4d6ccd343a6b298a2aa844f1bad66c736487251
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2020
ms.locfileid: "42591702"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var tokenIssuancePolicy = await graphClient.Policies.TokenIssuancePolicies["{id}"]
    .Request()
    .GetAsync();

```