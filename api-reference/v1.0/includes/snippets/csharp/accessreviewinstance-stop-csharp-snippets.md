---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 589941e1c21b7fd97b91ee6195bd875492d8f2ec
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/30/2021
ms.locfileid: "53211024"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.IdentityGovernance.AccessReviews.Definitions["{accessReviewScheduleDefinition-id}"].Instances["{accessReviewInstance-id}"]
    .Stop()
    .Request()
    .PostAsync();

```