---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4052f6705a121787cad0d64a5079bfef29e446aecd8c93b73dd1f3b7fdd15e7c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56898230"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.AccessReviews["{accessReview-id}"]
    .ResetDecisions()
    .Request()
    .PostAsync();

```