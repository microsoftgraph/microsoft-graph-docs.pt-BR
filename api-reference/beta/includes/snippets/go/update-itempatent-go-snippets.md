---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 886ab684e053fd3228e3d2a1a0a0adb833ccb97e
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61098333"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewItemPatent()
number := "USPTO-3954432633"
requestBody.SetNumber(&number)
webUrl := "https://patents.gov/3954432633"
requestBody.SetWebUrl(&webUrl)
options := &msgraphsdk.ItemPatentRequestBuilderPatchOptions{
    Body: requestBody,
}
userId := "user-id"
itemPatentId := "itemPatent-id"
graphClient.UsersById(&userId).Profile().PatentsById(&itemPatentId).Patch(options)


```