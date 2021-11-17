---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ee3fe46442a173e3d6d988a262ec131644036ff2
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61009117"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewApplication()
displayName := "Display name"
requestBody.SetDisplayName(&displayName)
options := &msgraphsdk.ApplicationsRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.Applications().Post(options)


```