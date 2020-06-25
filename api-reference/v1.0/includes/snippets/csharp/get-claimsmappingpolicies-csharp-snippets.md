---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 350ab9de9199754daf974cdf5bf7ea096ff27c1e
ms.sourcegitcommit: 1ec5a7be90790aaebdf6d85d93ab0c72b381c9c3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/24/2020
ms.locfileid: "44863284"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var claimsMappingPolicies = await graphClient.Policies.ClaimsMappingPolicies
    .Request()
    .GetAsync();

```