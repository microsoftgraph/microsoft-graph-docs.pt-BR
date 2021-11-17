---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d2dd0250fcdde5ee7f2b25c278b91e54e69701c3de8eb95b27a26289af72b1a7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57099832"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.AccessReviews["{accessReview-id}"]
    .ApplyDecisions()
    .Request()
    .PostAsync();

```