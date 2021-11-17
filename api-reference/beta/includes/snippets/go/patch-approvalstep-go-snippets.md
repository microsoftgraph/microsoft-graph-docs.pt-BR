---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 483215480ddf53b71cff964e24b2808115912036
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "60995340"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

approvalId := "approval-id"
approvalStepId := "approvalStep-id"
graphClient.IdentityGovernance().EntitlementManagement().AccessPackageAssignmentApprovalsById(&approvalId).StepsById(&approvalStepId).Patch(options)


```