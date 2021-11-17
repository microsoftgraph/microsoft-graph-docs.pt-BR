---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: dafd91098eedbcfd6b8463590327d40fc567af2cf5fa2e3ce09e1c0cb25f6540
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57217199"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var featureRolloutPolicy = await graphClient.Policies.FeatureRolloutPolicies["{featureRolloutPolicy-id}"]
    .Request()
    .GetAsync();

```