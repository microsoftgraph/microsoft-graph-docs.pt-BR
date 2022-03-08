---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: bd2f99f0ff5442b284b772bdc13e98927ed61428
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2022
ms.locfileid: "63333068"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.AccessPackageAssignmentPolicyRequestBuilderGetQueryParameters{
    Expand: "customExtensionHandlers($expand=customExtension)",
}
options := &msgraphsdk.AccessPackageAssignmentPolicyRequestBuilderGetOptions{
    Q: requestParameters,
}
accessPackageAssignmentPolicyId := "accessPackageAssignmentPolicy-id"
result, err := graphClient.IdentityGovernance().EntitlementManagement().AccessPackageAssignmentPoliciesById(&accessPackageAssignmentPolicyId).Get(options)


```