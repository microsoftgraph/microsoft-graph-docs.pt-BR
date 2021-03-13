---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 06d238f448bd1b726c806fa6ad8fa9685a014227
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50780857"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.IdentityGovernance.AccessReviews.Definitions["{accessReviewScheduleDefinition-id}"].Instances["{accessReviewInstance-id}"]
    .ApplyDecisions()
    .Request()
    .PostAsync();

```