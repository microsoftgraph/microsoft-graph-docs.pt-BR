---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: be0018358e01410e3ac263ea370693f8834eacb3
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61093753"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewStore()
defaultLanguageTag := "en-US"
requestBody.SetDefaultLanguageTag(&defaultLanguageTag)
options := &msgraphsdk.TermStoreRequestBuilderPatchOptions{
    Body: requestBody,
}
graphClient.TermStore().Patch(options)


```