---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f623cc42d27104fa0f9ef60013cba706f97e2cf2
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61285901"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

accessPackageAssignmentPolicyId := "accessPackageAssignmentPolicy-id"
graphClient.IdentityGovernance().EntitlementManagement().AccessPackageAssignmentPoliciesById(&accessPackageAssignmentPolicyId).Delete(nil)


```