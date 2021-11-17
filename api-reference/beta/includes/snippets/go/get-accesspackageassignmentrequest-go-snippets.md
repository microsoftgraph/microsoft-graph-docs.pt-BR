---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4d22a56f3104ffc4a2e69bc79df53791d0579727
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "60988241"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

accessPackageAssignmentRequestId := "accessPackageAssignmentRequest-id"
result, err := graphClient.IdentityGovernance().EntitlementManagement().AccessPackageAssignmentRequestsById(&accessPackageAssignmentRequestId).Get(options)


```