---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 42c4935a12c0bb82f88a47e3a0e5ccf4dc5aa7c8
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61286586"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

privilegedRoleAssignmentRequestId := "privilegedRoleAssignmentRequest-id"
result, err := graphClient.PrivilegedRoleAssignmentRequestsById(&privilegedRoleAssignmentRequestId).Get(nil)


```