---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fafec86ae88a24e2bccee9632bea7633c5c812dc
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "60984371"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

permissionGrantPolicyId := "permissionGrantPolicy-id"
result, err := graphClient.Policies().PermissionGrantPoliciesById(&permissionGrantPolicyId).Excludes().Get(options)


```