---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ae5336776c4d114b34e50ca23b9c1f3e9c9461a0
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61286329"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

plannerDeltaId := "plannerDelta-id"
result, err := graphClient.Me().Planner().AllById(&plannerDeltaId).Get(nil)


```