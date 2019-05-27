---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4cbe0d1663ecc301d7adb136b1a09f9eb9ba7b9a
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/25/2019
ms.locfileid: "34452026"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var accessReviewReviewer = new AccessReviewReviewer
{
    Id = "006111db-0810-4494-a6df-904d368bd81b"
};

await graphClient.AccessReviews["2b83cc42-09db-46f6-8c6e-16fec466a82d"].Reviewers
    .Request()
    .AddAsync(accessReviewReviewer);

```