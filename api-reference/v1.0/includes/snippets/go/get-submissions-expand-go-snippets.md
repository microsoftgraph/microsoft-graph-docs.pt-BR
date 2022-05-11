---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1120b08807536a6daadfd7cb30b7bdc65c35602c
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65324643"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.SubmissionsRequestBuilderGetQueryParameters{
    Expand: "outcomes",
}
options := &msgraphsdk.SubmissionsRequestBuilderGetRequestConfiguration{
    QueryParameters: requestParameters,
}
educationClassId := "educationClass-id"
educationAssignmentId := "educationAssignment-id"
result, err := graphClient.Education().ClassesById(&educationClassId).AssignmentsById(&educationAssignmentId).Submissions().GetWithRequestConfigurationAndResponseHandler(options, nil)


```