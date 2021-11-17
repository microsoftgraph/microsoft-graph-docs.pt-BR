---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 21647a80e3ee8095f6dc192851b53a4649844ea2
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "60988052"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

accessReviewId := "accessReview-id"
result, err := graphClient.AccessReviewsById(&accessReviewId).MyDecisions().Get(options)


```