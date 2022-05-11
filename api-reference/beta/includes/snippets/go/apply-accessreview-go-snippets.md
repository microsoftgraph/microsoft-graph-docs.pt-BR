---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e07869b2e8fd97c5cbc972bb7f9008eb72844299
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65322624"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

accessReviewId := "accessReview-id"
graphClient.AccessReviewsById(&accessReviewId).ApplyDecisions(accessReview-id).Post()


```