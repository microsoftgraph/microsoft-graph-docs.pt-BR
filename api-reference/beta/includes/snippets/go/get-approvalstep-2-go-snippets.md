---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f09761866ded03e9c9ff1c1aa1fc83d64292a3d5
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61285809"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

approvalId := "approval-id"
approvalStepId := "approvalStep-id"
result, err := graphClient.IdentityGovernance().EntitlementManagement().AccessPackageAssignmentApprovalsById(&approvalId).StepsById(&approvalStepId).Get(nil)


```