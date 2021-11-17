---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 476ec2b35c8de9ed12c013ee07a53264e48ce7c3
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "60984938"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.New()
password := "1234567890"
requestBody.SetPassword(&password)
options := &msgraphsdk.ValidatePasswordRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.Users().ValidatePassword().Post(options)


```