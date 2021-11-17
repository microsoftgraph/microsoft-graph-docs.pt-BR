---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: eec158a44a3b79405f0479d64d73f192f6728961
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61032161"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

privilegedRoleAssignmentRequestId := "privilegedRoleAssignmentRequest-id"
result, err := graphClient.PrivilegedRoleAssignmentRequestsById(&privilegedRoleAssignmentRequestId).Cancel().Post(options)


```