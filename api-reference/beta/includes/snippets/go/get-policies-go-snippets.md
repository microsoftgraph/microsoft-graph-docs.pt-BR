---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: efc0b809a106dfe6e0dfffa75ecdaec044129a7c
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65323241"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.PoliciesRequestBuilderGetQueryParameters{
    Filter: "displayName%20eq%20'SimplePolicy1'%20or%20displayName%20eq%20'SimplePolicy2'",
}
options := &msgraphsdk.PoliciesRequestBuilderGetRequestConfiguration{
    QueryParameters: requestParameters,
}
result, err := graphClient.Identity().ConditionalAccess().Policies().GetWithRequestConfigurationAndResponseHandler(options, nil)


```