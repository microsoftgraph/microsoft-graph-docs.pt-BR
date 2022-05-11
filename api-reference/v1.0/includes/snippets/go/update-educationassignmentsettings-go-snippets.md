---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 33737285965046f912104b39c629961f9e38cc60
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65322342"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewEducationAssignmentSettings()
submissionAnimationDisabled := true
requestBody.SetSubmissionAnimationDisabled(&submissionAnimationDisabled)
educationClassId := "educationClass-id"
graphClient.Education().ClassesById(&educationClassId).AssignmentSettings().Patch(requestBody)


```