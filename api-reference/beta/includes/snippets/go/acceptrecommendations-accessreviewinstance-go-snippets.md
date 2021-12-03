---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e5385b72aeb72607ceae0dc8527e1bff5f973500
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61285831"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

accessReviewInstanceId := "accessReviewInstance-id"
graphClient.Me().PendingAccessReviewInstancesById(&accessReviewInstanceId).AcceptRecommendations().Post(nil)


```