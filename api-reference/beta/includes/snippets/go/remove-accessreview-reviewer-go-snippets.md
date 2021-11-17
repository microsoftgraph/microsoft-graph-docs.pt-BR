---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b3aa6d86c24f0f8c1134ed5848ddf050c4e3f4e1
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "60988010"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

accessReviewId := "accessReview-id"
accessReviewReviewerId := "accessReviewReviewer-id"
graphClient.AccessReviewsById(&accessReviewId).ReviewersById(&accessReviewReviewerId).Delete(options)


```