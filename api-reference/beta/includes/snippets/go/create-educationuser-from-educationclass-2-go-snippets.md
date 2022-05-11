---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 3df618f5ebeb9771eb173800ab83bb5eaefc7503
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65325460"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.id": "https://graph.microsoft.com/beta/education/users/14011",
}
educationClassId := "educationClass-id"
educationUserId := "educationUser-id"
graphClient.Education().ClassesById(&educationClassId).TeachersById(&educationUserId).Post(requestBody)


```