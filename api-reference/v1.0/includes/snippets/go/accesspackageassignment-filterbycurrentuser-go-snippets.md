---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 023eed4f260d4b4e095b7ecbcff9695e26a8d1e0
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/08/2021
ms.locfileid: "61342873"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

accessPackageAssignmentId := "accessPackageAssignment-id"
result, err := graphClient.IdentityGovernance().EntitlementManagement().AssignmentsById(&accessPackageAssignmentId).Get(nil)


```