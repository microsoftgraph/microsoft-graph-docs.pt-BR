---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 13ece3b6e444cf9993404a9891f107fc3e658882
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/05/2022
ms.locfileid: "65211851"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

accessPackageAssignmentPolicyId := "accessPackageAssignmentPolicy-id"
graphClient.IdentityGovernance().EntitlementManagement().AssignmentPoliciesById(&accessPackageAssignmentPolicyId).Delete(nil)


```