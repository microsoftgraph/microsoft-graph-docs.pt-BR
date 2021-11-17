---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 586dc9ba729aa683ce65817a3cf97f3afecfdc15
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61001438"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewAdministrativeUnit()
displayName := "displayName-value"
requestBody.SetDisplayName(&displayName)
description := "description-value"
requestBody.SetDescription(&description)
visibility := "visibility-value"
requestBody.SetVisibility(&visibility)
options := &msgraphsdk.AdministrativeUnitRequestBuilderPatchOptions{
    Body: requestBody,
}
administrativeUnitId := "administrativeUnit-id"
graphClient.Directory().AdministrativeUnitsById(&administrativeUnitId).Patch(options)


```