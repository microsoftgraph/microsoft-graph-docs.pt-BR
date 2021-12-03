---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8cc2c241fa185d9aa8a18e7bb45b2f947be9219a
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61285885"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

accessReviewInstanceId := "accessReviewInstance-id"
accessReviewInstanceDecisionItemId := "accessReviewInstanceDecisionItem-id"
graphClient.Me().PendingAccessReviewInstancesById(&accessReviewInstanceId).DecisionsById(&accessReviewInstanceDecisionItemId).Patch(nil)


```