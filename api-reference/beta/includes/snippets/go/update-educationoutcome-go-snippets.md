---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1718a3b873d216b1d4f59bc341d348265b13e5ce
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/09/2022
ms.locfileid: "63411283"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewEducationOutcome()
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.type": "#microsoft.graph.educationRubricOutcome",
    "rubricQualityFeedback":  []Object {
    }
    "rubricQualitySelectedLevels":  []Object {
    }
}
options := &msgraphsdk.EducationOutcomeRequestBuilderPatchOptions{
    Body: requestBody,
}
educationClassId := "educationClass-id"
educationAssignmentId := "educationAssignment-id"
educationSubmissionId := "educationSubmission-id"
educationOutcomeId := "educationOutcome-id"
result, err := graphClient.Education().ClassesById(&educationClassId).AssignmentsById(&educationAssignmentId).SubmissionsById(&educationSubmissionId).OutcomesById(&educationOutcomeId).Patch(options)


```