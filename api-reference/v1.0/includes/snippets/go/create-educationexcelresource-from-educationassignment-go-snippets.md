---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a93da95dc3f9822113eea4013ced26cdb6f6572b
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61097927"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewEducationAssignmentResource()
distributeForStudentWork := false
requestBody.SetDistributeForStudentWork(&distributeForStudentWork)
resource := msgraphsdk.NewEducationResource()
requestBody.SetResource(resource)
displayName := "Graph Doc pages.xlsx"
resource.SetDisplayName(&displayName)
resource.SetAdditionalData(map[string]interface{}{
    "@odata.type": "microsoft.graph.educationExcelResource",
    "fileUrl": "https://graph.microsoft.com/v1.0/drives/b!OPmUsPgnBUiMIXMxWcj3neC1xck6I5NIsnFxfrLdmXoOOmEQNO79QpIMPdOmY3nf/items/01QTY63RIR7PSV4JJSFJHKNPUVUWGPW4O2",
}
options := &msgraphsdk.ResourcesRequestBuilderPostOptions{
    Body: requestBody,
}
educationClassId := "educationClass-id"
educationAssignmentId := "educationAssignment-id"
result, err := graphClient.Education().ClassesById(&educationClassId).AssignmentsById(&educationAssignmentId).Resources().Post(options)


```