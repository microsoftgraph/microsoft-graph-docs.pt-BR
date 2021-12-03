---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: dd0a06e2a5edde0e56eb2ee23f2b073bafebe9ab
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61285900"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

accessPackageAssignmentPolicyId := "accessPackageAssignmentPolicy-id"
result, err := graphClient.IdentityGovernance().EntitlementManagement().AccessPackageAssignmentPoliciesById(&accessPackageAssignmentPolicyId).Get(nil)


```