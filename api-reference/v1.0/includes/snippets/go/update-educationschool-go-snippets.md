---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: cd040ea7a74f071646fb9785648043dda4918330
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65322949"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewEducationSchool()
displayName := "Fabrikam Arts High School"
requestBody.SetDisplayName(&displayName)
description := "Magnate school for the arts. Los Angeles School District"
requestBody.SetDescription(&description)
educationSchoolId := "educationSchool-id"
graphClient.Education().SchoolsById(&educationSchoolId).Patch(requestBody)


```