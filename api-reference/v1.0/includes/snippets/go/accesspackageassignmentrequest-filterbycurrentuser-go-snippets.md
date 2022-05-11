---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 26445d95fe18531d504fb39e58a5861a8fc7a0f4
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65323690"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

accessPackageAssignmentRequestId := "accessPackageAssignmentRequest-id"
result, err := graphClient.IdentityGovernance().EntitlementManagement().AssignmentRequestsById(&accessPackageAssignmentRequestId).Get()


```