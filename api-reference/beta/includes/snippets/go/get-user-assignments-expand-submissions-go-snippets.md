---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a5de568342c035bc346375672642b7841370b3c7
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65322500"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.AssignmentsRequestBuilderGetQueryParameters{
    Expand: "submissions",
}
options := &msgraphsdk.AssignmentsRequestBuilderGetRequestConfiguration{
    QueryParameters: requestParameters,
}
educationUserId := "educationUser-id"
result, err := graphClient.Education().UsersById(&educationUserId).Assignments().GetWithRequestConfigurationAndResponseHandler(options, nil)


```