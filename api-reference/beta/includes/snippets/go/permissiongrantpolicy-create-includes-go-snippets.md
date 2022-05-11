---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f3887f19646c9041124c544c63b1c16c2873af41
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65323958"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewPermissionGrantConditionSet()
permissionType := "delegated"
requestBody.SetPermissionType(&permissionType)
certifiedClientApplicationsOnly := true
requestBody.SetCertifiedClientApplicationsOnly(&certifiedClientApplicationsOnly)
permissionGrantPolicyId := "permissionGrantPolicy-id"
result, err := graphClient.Policies().PermissionGrantPoliciesById(&permissionGrantPolicyId).Includes().Post(requestBody)


```