---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fd2e787f882e56314454b978abe4a53d8ea6ec3c
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50810185"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var accessReviewReviewer = new AccessReviewReviewer
{
    Id = "006111db-0810-4494-a6df-904d368bd81b"
};

await graphClient.AccessReviews["{accessReview-id}"].Reviewers
    .Request()
    .AddAsync(accessReviewReviewer);

```