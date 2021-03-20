---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d4dffa3848dbc16b8fd904e502526ac27fd7d762
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50943054"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.IdentityGovernance.AccessReviews.Definitions["{accessReviewScheduleDefinition-id}"].Instances["{accessReviewInstance-id}"]
    .SendReminder()
    .Request()
    .PostAsync();

```