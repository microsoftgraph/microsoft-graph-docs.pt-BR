---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9116a1fbc4c6c700b37075d6a39f25abb0286863
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/09/2022
ms.locfileid: "63671353"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

privilegedRoleAssignmentRequestId := "privilegedRoleAssignmentRequest-id"
result, err := graphClient.PrivilegedRoleAssignmentRequestsById(&privilegedRoleAssignmentRequestId).Cancel(privilegedRoleAssignmentRequest-id).Post(nil)


```