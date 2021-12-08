---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 3a70f3ce8011c7fad01d72c3d7242a935c5db046
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/08/2021
ms.locfileid: "61334568"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

accessPackageAssignmentRequestId := "accessPackageAssignmentRequest-id"
graphClient.IdentityGovernance().EntitlementManagement().AssignmentRequestsById(&accessPackageAssignmentRequestId).Delete(nil)


```