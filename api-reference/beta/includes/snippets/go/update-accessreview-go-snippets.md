---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: da19379952cd21ac6abf406baa945e1bcd3d4170
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61087542"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewAccessReview()
displayName := "TestReview new name"
requestBody.SetDisplayName(&displayName)
options := &msgraphsdk.AccessReviewRequestBuilderPatchOptions{
    Body: requestBody,
}
accessReviewId := "accessReview-id"
graphClient.AccessReviewsById(&accessReviewId).Patch(options)


```