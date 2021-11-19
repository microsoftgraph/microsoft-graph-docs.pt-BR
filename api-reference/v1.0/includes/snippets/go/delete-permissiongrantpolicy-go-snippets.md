---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9971f2fa12690a8363f5436d05873c07cbd329ec
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61092337"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

permissionGrantPolicyId := "permissionGrantPolicy-id"
graphClient.Policies().PermissionGrantPoliciesById(&permissionGrantPolicyId).Delete(options)


```