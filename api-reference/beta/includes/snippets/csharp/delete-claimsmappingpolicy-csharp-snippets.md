---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 89df40172cbdc475a2032f71edd85193f9028186
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50806265"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Policies.ClaimsMappingPolicies["{claimsMappingPolicy-id}"]
    .Request()
    .DeleteAsync();

```