---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: caf414270f5a162d798acd983732f32d2f2f9c8b
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61022368"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewDriveItem()
name := "My Day at the Beach"
requestBody.SetName(&name)
bundle := msgraphsdk.NewBundle()
requestBody.SetBundle(bundle)
album := msgraphsdk.NewAlbum()
bundle.SetAlbum(album)
requestBody.SetChildren( []DriveItem {
    msgraphsdk.NewDriveItem(),
    SetAdditionalData(map[string]interface{}{
        "id": "1234asdf",
    }
}
requestBody.SetAdditionalData(map[string]interface{}{
    "@microsoft.graph.conflictBehavior": "rename",
}
options := &msgraphsdk.BundlesRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.Drive().Bundles().Post(options)


```