---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9414a68f1830becf251e4c75d6161c9b127ed27f
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/09/2022
ms.locfileid: "63411342"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.id": "https://graph.microsoft.com/v1.0/groups/{id}",
}
options := &msgraphsdk.DirectoryObjectRequestBuilderPostOptions{
    Body: requestBody,
}
administrativeUnitId := "administrativeUnit-id"
directoryObjectId := "directoryObject-id"
graphClient.Directory().AdministrativeUnitsById(&administrativeUnitId).MembersById(&directoryObjectId).Post(options)


```