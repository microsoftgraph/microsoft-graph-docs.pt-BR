---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 21727d27b73d96ee183299cc0bb09678a1558466
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65322637"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.AccessPackageAssignmentPolicyRequestBuilderGetQueryParameters{
    Expand: "customExtensionHandlers($expand=customExtension)",
}
options := &msgraphsdk.AccessPackageAssignmentPolicyRequestBuilderGetRequestConfiguration{
    QueryParameters: requestParameters,
}
accessPackageAssignmentPolicyId := "accessPackageAssignmentPolicy-id"
result, err := graphClient.IdentityGovernance().EntitlementManagement().AccessPackageAssignmentPoliciesById(&accessPackageAssignmentPolicyId).GetWithRequestConfigurationAndResponseHandler(options, nil)


```