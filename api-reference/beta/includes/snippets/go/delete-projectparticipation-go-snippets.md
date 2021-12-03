---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: df699b241128002a494e2b60a59ba418ebf62b8c
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61286734"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

projectParticipationId := "projectParticipation-id"
graphClient.Me().Profile().ProjectsById(&projectParticipationId).Delete(nil)


```