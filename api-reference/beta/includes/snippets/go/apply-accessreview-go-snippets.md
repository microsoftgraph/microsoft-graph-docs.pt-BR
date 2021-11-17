---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2d39d39ff55716b471943f9991088f9a2e727736
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "60983096"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

accessReviewId := "accessReview-id"
graphClient.AccessReviewsById(&accessReviewId).ApplyDecisions().Post(options)


```