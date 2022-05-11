---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 25ddcec4ca5b415a17f7fa955d86b89779601df5
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65322703"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
requestBody.SetAdditionalData(map[string]interface{}{
    "baseType": "microsoft.graph.externalItem",
    "properties":  []Object {
    }
}
externalConnectionId := "externalConnection-id"
graphClient.External().ConnectionsById(&externalConnectionId).Schema().Post(requestBody)


```