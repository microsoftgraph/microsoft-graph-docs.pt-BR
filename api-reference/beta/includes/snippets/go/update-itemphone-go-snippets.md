---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b6f59775414b937ee301e7a5020ceb8fdef89af3
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "60981235"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewItemPhone()
type := "other"
requestBody.SetType(&type)
options := &msgraphsdk.ItemPhoneRequestBuilderPatchOptions{
    Body: requestBody,
}
userId := "user-id"
itemPhoneId := "itemPhone-id"
graphClient.UsersById(&userId).Profile().PhonesById(&itemPhoneId).Patch(options)


```