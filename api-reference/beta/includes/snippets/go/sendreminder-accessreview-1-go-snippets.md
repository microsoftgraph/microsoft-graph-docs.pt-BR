---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 98f0840992b049e8a5acdc3b2d71a3e3f013e378
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61091157"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

accessReviewId := "accessReview-id"
graphClient.AccessReviewsById(&accessReviewId).SendReminder().Post(options)


```