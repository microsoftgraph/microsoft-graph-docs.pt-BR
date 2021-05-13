---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f726c8f3207b8ceea41d3b2ee00b288465bb20ea
ms.sourcegitcommit: b8b0e88b3ba9a434dc45f5ab640cb46f66fae299
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/13/2021
ms.locfileid: "52474215"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.IdentityGovernance.AccessReviews.HistoryDefinitions["{accessReviewHistoryDefinition-id}"]
    .GenerateDownloadUri()
    .Request()
    .PostAsync();

```