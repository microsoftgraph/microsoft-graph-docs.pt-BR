---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 46202feede5249e00630e0376a993e51df9be751
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/09/2022
ms.locfileid: "63395528"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
requestBody.SetAdditionalData(map[string]interface{}{
    "id": "123456!87",
}
options := &msgraphsdk.ChildrenRequestBuilderPostOptions{
    Body: requestBody,
}
driveItemId := "driveItem-id"
graphClient.Drive().BundlesById(&driveItemId).Children().Post(options)


```