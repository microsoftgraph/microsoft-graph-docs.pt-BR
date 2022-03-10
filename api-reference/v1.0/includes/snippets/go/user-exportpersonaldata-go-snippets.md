---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9567ec4205bea8432226e8498062d40cbc1f2552
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/09/2022
ms.locfileid: "63411290"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewStorageLocationRequestBody()
storageLocation := "storageLocation-value"
requestBody.SetStorageLocation(&storageLocation)
options := &msgraphsdk.ExportPersonalDataRequestBuilderPostOptions{
    Body: requestBody,
}
userId := "user-id"
graphClient.UsersById(&userId).ExportPersonalData(user-id).Post(options)


```