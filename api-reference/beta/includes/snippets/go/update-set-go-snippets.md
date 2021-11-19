---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b19b17461d8d99d011cb3b4e45ab168776a4a0bc
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61085452"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewSet()
description := "mySet"
requestBody.SetDescription(&description)
options := &msgraphsdk.SetRequestBuilderPatchOptions{
    Body: requestBody,
}
setId := "set-id"
graphClient.TermStore().SetsById(&setId).Patch(options)


```