---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 642e40e1764d8025ccd976ca44813b036872254b
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "60994576"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.New()
role := "viewer"
requestBody.SetRole(&role)
options := &msgraphsdk.ChangeScreenSharingRoleRequestBuilderPostOptions{
    Body: requestBody,
}
callId := "call-id"
graphClient.Communications().CallsById(&callId).ChangeScreenSharingRole().Post(options)


```