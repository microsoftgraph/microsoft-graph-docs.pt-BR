---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 899002e48151deda15280da268f23c5f1ad3fea0
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61008332"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewUser()
requestBody.SetBusinessPhones( []String {
    "+1 425 555 0109",
}
officeLocation := "18/2111"
requestBody.SetOfficeLocation(&officeLocation)
options := &msgraphsdk.UserRequestBuilderPatchOptions{
    Body: requestBody,
}
userId := "user-id"
graphClient.UsersById(&userId).Patch(options)


```