---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ee880af1df23a0605868479ffa914fc32927a15c
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/05/2022
ms.locfileid: "65207306"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

result, err := graphClient.RoleManagement().Directory().RoleAssignmentScheduleInstances().Get(nil)


```