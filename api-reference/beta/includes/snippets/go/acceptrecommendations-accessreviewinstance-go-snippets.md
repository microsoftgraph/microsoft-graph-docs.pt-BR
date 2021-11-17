---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ac322dda846e3868e4cd2d1de5d75d2cc7a4b0dd
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "60992022"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

accessReviewInstanceId := "accessReviewInstance-id"
graphClient.Me().PendingAccessReviewInstancesById(&accessReviewInstanceId).AcceptRecommendations().Post(options)


```