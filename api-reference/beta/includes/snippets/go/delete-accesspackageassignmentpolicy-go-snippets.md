---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c007c36da71f242127d836af28f59a0af4cadedc
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65322639"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

accessPackageAssignmentPolicyId := "accessPackageAssignmentPolicy-id"
graphClient.IdentityGovernance().EntitlementManagement().AccessPackageAssignmentPoliciesById(&accessPackageAssignmentPolicyId).Delete()


```