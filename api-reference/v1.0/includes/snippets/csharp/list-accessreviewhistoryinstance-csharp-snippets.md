---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 394867ccc46b7847086c35e2cfb975d8f7829350
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2022
ms.locfileid: "63337564"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var instances = await graphClient.IdentityGovernance.AccessReviews.HistoryDefinitions["{accessReviewHistoryDefinition-id}"].Instances
    .Request()
    .GetAsync();

```