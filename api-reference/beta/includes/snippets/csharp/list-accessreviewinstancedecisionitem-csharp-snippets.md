---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b4b92efe68d781b5c8719d3a70ad4fe5a89d70ac
ms.sourcegitcommit: ada6eab637b9b318129aefb98edbe7316399d9ba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/07/2021
ms.locfileid: "53319552"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var decisions = await graphClient.IdentityGovernance.AccessReviews.Definitions["{accessReviewScheduleDefinition-id}"].Instances["{accessReviewInstance-id}"].Decisions
    .Request()
    .GetAsync();

```