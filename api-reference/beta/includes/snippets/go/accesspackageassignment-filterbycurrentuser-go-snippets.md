---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ad9403a9c73147cf133e4c7052276ebb1fe99b74
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "60983608"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

accessPackageAssignmentId := "accessPackageAssignment-id"
result, err := graphClient.IdentityGovernance().EntitlementManagement().AccessPackageAssignmentsById(&accessPackageAssignmentId).Get(options)


```