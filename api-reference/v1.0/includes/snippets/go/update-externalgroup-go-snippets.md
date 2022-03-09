---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9c66943434b51f59dc15d8bfa0af776741d277eb
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/09/2022
ms.locfileid: "63395269"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewExternalGroup()
displayName := "Contoso Marketing"
requestBody.SetDisplayName(&displayName)
description := "The product marketing team"
requestBody.SetDescription(&description)
options := &msgraphsdk.ExternalGroupRequestBuilderPatchOptions{
    Body: requestBody,
}
externalConnectionId := "externalConnection-id"
externalGroupId := "externalGroup-id"
result, err := graphClient.External().ConnectionsById(&externalConnectionId).GroupsById(&externalGroupId).Patch(options)


```