---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 0239ed3022122b3ce9d2b1c46bfc5b5021b57019
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/09/2022
ms.locfileid: "63410499"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewPasswordRequestBody()
password := "1234567890"
requestBody.SetPassword(&password)
options := &msgraphsdk.ValidatePasswordRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.Users().ValidatePassword().Post(options)


```