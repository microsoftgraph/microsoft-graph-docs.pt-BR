---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 45dd779578142d837576051a6edbc9c465d2fe05
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/02/2021
ms.locfileid: "51508895"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Policies.FeatureRolloutPolicies["{featureRolloutPolicy-id}"]
    .Request()
    .DeleteAsync();

```