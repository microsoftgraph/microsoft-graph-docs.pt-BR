---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 167a0a5428214b69502bf3612ef720e21cd03c9d
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61091350"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
password := "1234567890"
requestBody.SetPassword(&password)
options := &msgraphsdk.ValidatePasswordRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.Users().ValidatePassword().Post(options)


```