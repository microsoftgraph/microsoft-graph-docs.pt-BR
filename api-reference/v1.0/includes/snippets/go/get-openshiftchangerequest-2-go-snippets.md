---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 1ad2d2abbf28ae509f7aebd179f7e9f621b87cd3
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61287229"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

teamId := "team-id"
result, err := graphClient.TeamsById(&teamId).Schedule().OpenShiftChangeRequests().Get(nil)


```