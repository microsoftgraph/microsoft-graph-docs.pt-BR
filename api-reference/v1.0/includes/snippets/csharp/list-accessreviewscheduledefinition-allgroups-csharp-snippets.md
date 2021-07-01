---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ee32be76a31b369cc2ff1c261b580a70c12ad69b
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/30/2021
ms.locfileid: "53208688"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var definitions = await graphClient.IdentityGovernance.AccessReviews.Definitions
    .Request()
    .Filter("contains(scope/microsoft.graph.accessReviewQueryScope/query, './members')")
    .GetAsync();

```