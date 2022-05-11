---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 3ea6e6009875b902c03ebbe934053b20e8a9b779
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65324662"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewProfileCardProperty()
directoryPropertyName := "CustomAttribute1"
requestBody.SetDirectoryPropertyName(&directoryPropertyName)
requestBody.SetAnnotations( []ProfileCardAnnotation {
    msgraphsdk.NewProfileCardAnnotation(),
    SetAdditionalData(map[string]interface{}{
        "displayName": "Cost Center",
        "localizations":  []Object {
        }
    }
}
organizationId := "organization-id"
result, err := graphClient.OrganizationById(&organizationId).Settings().ProfileCardProperties().Post(requestBody)


```