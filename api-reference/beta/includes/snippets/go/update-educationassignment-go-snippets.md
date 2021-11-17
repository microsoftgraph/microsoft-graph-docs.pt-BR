---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8fed87bd189e6040d128100a5f27d3f268b10ff2
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61003145"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewEducationAssignment()
displayName := "Reading and review test 09.03 #5"
requestBody.SetDisplayName(&displayName)
instructions := msgraphsdk.NewEducationItemBody()
requestBody.SetInstructions(instructions)
contentType := "text"
instructions.SetContentType(&contentType)
content := "Read chapter 5 and write your review"
instructions.SetContent(&content)
dueDateTime, err := time.Parse(time.RFC3339, "2021-09-10T00:00:00Z")
requestBody.SetDueDateTime(&dueDateTime)
addedStudentAction := "none"
requestBody.SetAddedStudentAction(&addedStudentAction)
addToCalendarAction := "studentsAndPublisher"
requestBody.SetAddToCalendarAction(&addToCalendarAction)
options := &msgraphsdk.EducationAssignmentRequestBuilderPatchOptions{
    Body: requestBody,
}
educationClassId := "educationClass-id"
educationAssignmentId := "educationAssignment-id"
graphClient.Education().ClassesById(&educationClassId).AssignmentsById(&educationAssignmentId).Patch(options)


```