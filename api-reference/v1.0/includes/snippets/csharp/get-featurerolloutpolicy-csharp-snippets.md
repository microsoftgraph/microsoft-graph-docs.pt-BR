---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d9d973e0a6a49018ddc8186712d51d7d15c4f19d
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/25/2021
ms.locfileid: "51201385"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var featureRolloutPolicy = await graphClient.Policies.FeatureRolloutPolicies["{featureRolloutPolicy-id}"]
    .Request()
    .GetAsync();

```