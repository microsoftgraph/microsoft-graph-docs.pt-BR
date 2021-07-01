---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c0d7cb4e951af367f7f1d3abf08c550ee4b0b235
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/30/2021
ms.locfileid: "53208647"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var accessReviewScheduleDefinition = await graphClient.IdentityGovernance.AccessReviews.Definitions["{accessReviewScheduleDefinition-id}"]
    .Request()
    .GetAsync();

```