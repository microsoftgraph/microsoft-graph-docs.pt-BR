---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e843c20489eaf390de57b7ce058561bf226e6019
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/02/2021
ms.locfileid: "51507199"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var accessReviewInstanceDecisionItem = new AccessReviewInstanceDecisionItem
{
    Decision = "Approve",
    Justification = "This person is still on my team"
};

await graphClient.Me.PendingAccessReviewInstances["{accessReviewInstance-id}"].Decisions["{accessReviewInstanceDecisionItem-id}"]
    .Request()
    .UpdateAsync(accessReviewInstanceDecisionItem);

```