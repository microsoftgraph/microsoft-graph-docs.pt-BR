---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ef4f6c4b84bae9c45d5b2b7996d524f5e318b09c
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61084058"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

permissionGrantPolicyId := "permissionGrantPolicy-id"
permissionGrantConditionSetId := "permissionGrantConditionSet-id"
graphClient.Policies().PermissionGrantPoliciesById(&permissionGrantPolicyId).IncludesById(&permissionGrantConditionSetId).Delete(options)


```