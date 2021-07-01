---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a49d65bf5483b82d010fe0cbfea046c2cfe539bb
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/30/2021
ms.locfileid: "53209756"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.IdentityGovernance.AccessReviews.Definitions["{accessReviewScheduleDefinition-id}"].Instances["{accessReviewInstance-id}"]
    .ResetDecisions()
    .Request()
    .PostAsync();

```