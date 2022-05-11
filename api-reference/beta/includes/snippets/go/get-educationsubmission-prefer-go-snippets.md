---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 48809c91a3411f620082f69b53f794b3366452b8
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65325383"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

headers := map[string]string{
    "Prefer": "include-unknown-enum-members"
}
options := &msgraphsdk.EducationSubmissionRequestBuilderGetRequestConfiguration{
    Headers: headers,
}
educationClassId := "educationClass-id"
educationAssignmentId := "educationAssignment-id"
educationSubmissionId := "educationSubmission-id"
result, err := graphClient.Education().ClassesById(&educationClassId).AssignmentsById(&educationAssignmentId).SubmissionsById(&educationSubmissionId).GetWithRequestConfigurationAndResponseHandler(options, nil)


```