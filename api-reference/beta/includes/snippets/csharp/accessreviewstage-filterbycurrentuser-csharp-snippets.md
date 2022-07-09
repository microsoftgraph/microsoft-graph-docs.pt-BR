---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 53087000571c7e4651638e795a671baa46e70074
ms.sourcegitcommit: 6968f5aaf40089684efb0c38a95f6cca353c1d92
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/16/2022
ms.locfileid: "62854144"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var filterByCurrentUser = await graphClient.IdentityGovernance.AccessReviews.Definitions["{accessReviewScheduleDefinition-id}"].Instances["{accessReviewInstance-id}"].Stages
    .FilterByCurrentUser(AccessReviewStageFilterByCurrentUserOptions.Reviewer)
    .Request()
    .GetAsync();

```