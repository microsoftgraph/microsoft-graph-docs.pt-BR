---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ed2f4e853ad9db69c17bce861b9c54f767570225
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61286575"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

permissionGrantPolicyId := "permissionGrantPolicy-id"
permissionGrantConditionSetId := "permissionGrantConditionSet-id"
graphClient.Policies().PermissionGrantPoliciesById(&permissionGrantPolicyId).ExcludesById(&permissionGrantConditionSetId).Delete(nil)


```