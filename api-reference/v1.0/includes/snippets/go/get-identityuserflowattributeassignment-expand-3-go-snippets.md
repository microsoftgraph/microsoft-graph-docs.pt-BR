---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 333e1b8daf3e1792364f9b7b0b7fc7b83afdb81f
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65323665"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.IdentityUserFlowAttributeAssignmentRequestBuilderGetQueryParameters{
    Expand: "userAttribute",
}
options := &msgraphsdk.IdentityUserFlowAttributeAssignmentRequestBuilderGetRequestConfiguration{
    QueryParameters: requestParameters,
}
b2xIdentityUserFlowId := "b2xIdentityUserFlow-id"
identityUserFlowAttributeAssignmentId := "identityUserFlowAttributeAssignment-id"
result, err := graphClient.Identity().B2xUserFlowsById(&b2xIdentityUserFlowId).UserAttributeAssignmentsById(&identityUserFlowAttributeAssignmentId).GetWithRequestConfigurationAndResponseHandler(options, nil)


```