---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a728a0f0bb3c821b67318e24370685af2bb99320
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61005077"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.New()
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.id": "https://graph.microsoft.com/beta/education/classes/11006",
}
options := &msgraphsdk.RefRequestBuilderPostOptions{
    Body: requestBody,
}
educationSchoolId := "educationSchool-id"
result, err := graphClient.Education().SchoolsById(&educationSchoolId).Classes().$ref().Post(options)


```