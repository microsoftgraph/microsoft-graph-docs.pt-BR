---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 589941e1c21b7fd97b91ee6195bd875492d8f2ec
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50808467"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.IdentityGovernance.AccessReviews.Definitions["{accessReviewScheduleDefinition-id}"].Instances["{accessReviewInstance-id}"]
    .Stop()
    .Request()
    .PostAsync();

```