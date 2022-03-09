---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f700c7850332e0d4e10b2c27634b3f0faa545551
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/09/2022
ms.locfileid: "63396788"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
requestBody.SetAdditionalData(map[string]interface{}{
    "acl":  []Object {
    }
}
options := &msgraphsdk.ExternalItemRequestBuilderPutOptions{
    Body: requestBody,
}
externalConnectionId := "externalConnection-id"
externalItemId := "externalItem-id"
graphClient.External().ConnectionsById(&externalConnectionId).ItemsById(&externalItemId).Put(options)


```