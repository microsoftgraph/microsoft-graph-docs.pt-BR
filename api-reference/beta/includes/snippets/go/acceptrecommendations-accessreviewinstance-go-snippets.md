---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1acf062e51c6049dbc05cf987e1734700ab215a6
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65322615"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

accessReviewInstanceId := "accessReviewInstance-id"
graphClient.Me().PendingAccessReviewInstancesById(&accessReviewInstanceId).AcceptRecommendations(accessReviewInstance-id).Post()


```