---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 76bf8d03cb1f2081acce09566c337edd9befae59
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65325067"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewUser()
requestBody.SetBusinessPhones( []String {
    "+1 425 555 0109",
}
officeLocation := "18/2111"
requestBody.SetOfficeLocation(&officeLocation)
userId := "user-id"
graphClient.UsersById(&userId).Patch(requestBody)


```