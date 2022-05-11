---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5912297287fe775dd8821f17c22fc154f4181731
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65323075"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

accessPackageAssignmentPolicyId := "accessPackageAssignmentPolicy-id"
result, err := graphClient.IdentityGovernance().EntitlementManagement().AssignmentPoliciesById(&accessPackageAssignmentPolicyId).Get()


```