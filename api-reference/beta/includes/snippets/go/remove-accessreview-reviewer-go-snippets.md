---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 831252362e79648239dc22b6f3f5a51b465feab1
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61090813"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

accessReviewId := "accessReview-id"
accessReviewReviewerId := "accessReviewReviewer-id"
graphClient.AccessReviewsById(&accessReviewId).ReviewersById(&accessReviewReviewerId).Delete(options)


```