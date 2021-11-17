---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 829c7308437ed1917eedfc57c93126a0fce73000
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61029887"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewWorkPosition()
isCurrent := true
requestBody.SetIsCurrent(&isCurrent)
options := &msgraphsdk.WorkPositionRequestBuilderPatchOptions{
    Body: requestBody,
}
workPositionId := "workPosition-id"
graphClient.Me().Profile().PositionsById(&workPositionId).Patch(options)


```