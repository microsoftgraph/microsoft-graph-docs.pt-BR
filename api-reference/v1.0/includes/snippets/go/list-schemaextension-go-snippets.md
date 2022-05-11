---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 63041dafdf362d19643f9a343f56a16f17f585fd
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65325078"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.UsersRequestBuilderGetQueryParameters{
    Select: "ext55gb1l09_msLearnCourses",
}
options := &msgraphsdk.UsersRequestBuilderGetRequestConfiguration{
    QueryParameters: requestParameters,
}
result, err := graphClient.Users().GetWithRequestConfigurationAndResponseHandler(options, nil)


```