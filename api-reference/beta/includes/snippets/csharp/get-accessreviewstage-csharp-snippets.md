---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 84f4418884ae342435762ecc27cde179afdc120d
ms.sourcegitcommit: 6968f5aaf40089684efb0c38a95f6cca353c1d92
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/16/2022
ms.locfileid: "62853325"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var accessReviewStage = await graphClient.IdentityGovernance.AccessReviews.Definitions["{accessReviewScheduleDefinition-id}"].Instances["{accessReviewInstance-id}"].Stages["{accessReviewStage-id}"]
    .Request()
    .GetAsync();

```