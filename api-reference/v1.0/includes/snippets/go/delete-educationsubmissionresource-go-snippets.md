---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c48eca28676cc84bc023bd8f7e6cd3c2d5974630
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/09/2022
ms.locfileid: "63410793"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

educationClassId := "educationClass-id"
educationAssignmentId := "educationAssignment-id"
educationSubmissionId := "educationSubmission-id"
educationSubmissionResourceId := "educationSubmissionResource-id"
result, err := graphClient.Education().ClassesById(&educationClassId).AssignmentsById(&educationAssignmentId).SubmissionsById(&educationSubmissionId).ResourcesById(&educationSubmissionResourceId).Delete(nil)


```