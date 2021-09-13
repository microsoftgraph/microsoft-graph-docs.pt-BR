---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: daf2a3d479df691115138bc139a8eebb5165b0e91c9b1b5d9e18616577436564
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57273467"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Policies.FeatureRolloutPolicies["{featureRolloutPolicy-id}"]
    .Request()
    .DeleteAsync();

```