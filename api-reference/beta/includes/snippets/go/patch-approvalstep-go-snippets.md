---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 151f069712439c99cfd60b4229de94bd9b24fc02
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65323141"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

approvalId := "approval-id"
approvalStepId := "approvalStep-id"
graphClient.IdentityGovernance().EntitlementManagement().AccessPackageAssignmentApprovalsById(&approvalId).StepsById(&approvalStepId).Patch()


```