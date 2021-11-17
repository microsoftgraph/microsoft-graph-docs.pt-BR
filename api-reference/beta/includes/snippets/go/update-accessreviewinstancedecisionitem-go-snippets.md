---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: caf58ebc4960476a879d5c0c15331c91aaf38ca5
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "60987717"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

accessReviewInstanceId := "accessReviewInstance-id"
accessReviewInstanceDecisionItemId := "accessReviewInstanceDecisionItem-id"
graphClient.Me().PendingAccessReviewInstancesById(&accessReviewInstanceId).DecisionsById(&accessReviewInstanceDecisionItemId).Patch(options)


```