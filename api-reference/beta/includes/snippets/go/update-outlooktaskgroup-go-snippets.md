---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2dbff5feec28c9569f0a138c128c1d28bc6ba47f
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61286566"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

outlookTaskGroupId := "outlookTaskGroup-id"
graphClient.Me().Outlook().TaskGroupsById(&outlookTaskGroupId).Patch(nil)


```