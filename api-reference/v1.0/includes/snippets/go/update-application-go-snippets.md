---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 12e2bae94b77522248987fcc2c1f39539dc241ac
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61082935"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewApplication()
displayName := "New display name"
requestBody.SetDisplayName(&displayName)
options := &msgraphsdk.ApplicationRequestBuilderPatchOptions{
    Body: requestBody,
}
applicationId := "application-id"
graphClient.ApplicationsById(&applicationId).Patch(options)


```