---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9059eb05a954dee85f4d938ff72382506af3a2f7
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61098542"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

accessReviewId := "accessReview-id"
result, err := graphClient.AccessReviewsById(&accessReviewId).MyDecisions().Get(options)


```