---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 53d05d610a2a7898347189d4ea849c651c5ceb88
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50801881"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var reviewers = await graphClient.AccessReviews["{accessReview-id}"].Reviewers
    .Request()
    .GetAsync();

```