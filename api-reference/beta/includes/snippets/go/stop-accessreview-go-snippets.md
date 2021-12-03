---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 68d956c59bdbf041fefc7571c9cbad05ace060ac
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61285834"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

accessReviewId := "accessReview-id"
graphClient.AccessReviewsById(&accessReviewId).Stop().Post(nil)


```