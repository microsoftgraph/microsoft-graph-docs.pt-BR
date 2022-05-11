---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7ed738c3a89832ed299d5a7ed97c7d88cd3e6ac8
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65324329"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewPermissionGrantConditionSet()
permissionType := "delegated"
requestBody.SetPermissionType(&permissionType)
resourceApplication := "00000003-0000-0000-c000-000000000000"
requestBody.SetResourceApplication(&resourceApplication)
permissionGrantPolicyId := "permissionGrantPolicy-id"
result, err := graphClient.Policies().PermissionGrantPoliciesById(&permissionGrantPolicyId).Excludes().Post(requestBody)


```