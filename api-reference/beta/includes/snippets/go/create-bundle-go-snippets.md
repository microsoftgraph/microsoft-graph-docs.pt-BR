---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d4df3f9e10ebb38770749cf238a8345a57cd4e6c
ms.sourcegitcommit: 0d6d39dd6450e0c5fd6844cb78aead00a0782e46
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2022
ms.locfileid: "63759312"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
requestBody.SetAdditionalData(map[string]interface{}{
    "name": "Just some files",
    "@microsoft.graph.conflictBehavior": "rename",
    "children":  []Object {
    }
}
options := &msgraphsdk.BundlesRequestBuilderPostOptions{
    Body: requestBody,
}
graphClient.Drive().Bundles().Post(options)


```