---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5d5c689129cd0a2162623ffa16621eae626da957
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65324798"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.GroupsRequestBuilderGetQueryParameters{
    Filter: "mailEnabled%20eq%20false%20and%20securityEnabled%20eq%20true%20and%20NOT(groupTypes/any(s:s%20eq%20'Unified'))%20and%20membershipRuleProcessingState%20eq%20'On'",
    Count: true,
    Select: "id,membershipRule,membershipRuleProcessingState",
}
options := &msgraphsdk.GroupsRequestBuilderGetRequestConfiguration{
    QueryParameters: requestParameters,
}
result, err := graphClient.Groups().GetWithRequestConfigurationAndResponseHandler(options, nil)


```