---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 66b6021c9d8b260c6a05c6a013e48827de347196
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/03/2022
ms.locfileid: "62340544"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.IdentityGovernance.AccessReviews.HistoryDefinitions["{accessReviewHistoryDefinition-id}"].Instances["{accessReviewHistoryInstance-id}"]
    .GenerateDownloadUri()
    .Request()
    .PostAsync();

```