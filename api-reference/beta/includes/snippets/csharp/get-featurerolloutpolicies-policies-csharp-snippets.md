---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 0daba81328ad4d440c4fb29044600e2d78fbb0feb1ac1b5ef8ad0ca032bcaff1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57158801"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var featureRolloutPolicies = await graphClient.Policies.FeatureRolloutPolicies
    .Request()
    .GetAsync();

```