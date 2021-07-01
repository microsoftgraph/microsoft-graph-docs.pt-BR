---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c71602dc934c8f9f2e454c4fad287dc0d68d1623
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/30/2021
ms.locfileid: "53209610"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var accessReviewInstanceDecisionItem = new AccessReviewInstanceDecisionItem
{
    Decision = "Approve",
    Justification = "Kathleen still needs access to the Marketing group as she works in the Marketing organization."
};

await graphClient.IdentityGovernance.AccessReviews.Definitions["{accessReviewScheduleDefinition-id}"].Instances["{accessReviewInstance-id}"].Decisions["{accessReviewInstanceDecisionItem-id}"]
    .Request()
    .UpdateAsync(accessReviewInstanceDecisionItem);

```