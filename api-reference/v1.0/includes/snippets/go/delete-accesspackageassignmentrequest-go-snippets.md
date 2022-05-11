---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 26d3d9e54dbdd0a9074534bd8e2df9810f70dc70
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65323416"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

accessPackageAssignmentRequestId := "accessPackageAssignmentRequest-id"
graphClient.IdentityGovernance().EntitlementManagement().AssignmentRequestsById(&accessPackageAssignmentRequestId).Delete()


```