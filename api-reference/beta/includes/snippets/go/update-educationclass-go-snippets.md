---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 531ac8192cc420c73e234142cd7640ff1bbeb0b1
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62106245"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewEducationClass()
description := "History - World History 1"
requestBody.SetDescription(&description)
displayName := "World History Level 1"
requestBody.SetDisplayName(&displayName)
options := &msgraphsdk.EducationClassRequestBuilderPatchOptions{
    Body: requestBody,
}
educationClassId := "educationClass-id"
graphClient.Education().ClassesById(&educationClassId).Patch(options)


```