---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 01fd21356cf50bb3e20f5f9271b85bd48999378d
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/09/2022
ms.locfileid: "63410795"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewEducationSchool()
displayName := "Fabrikam Arts High School"
requestBody.SetDisplayName(&displayName)
description := "Magnate school for the arts. Los Angeles School District"
requestBody.SetDescription(&description)
options := &msgraphsdk.EducationSchoolRequestBuilderPatchOptions{
    Body: requestBody,
}
educationSchoolId := "educationSchool-id"
result, err := graphClient.Education().SchoolsById(&educationSchoolId).Patch(options)


```