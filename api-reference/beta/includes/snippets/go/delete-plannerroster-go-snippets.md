---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 43470d951ad28504645b69d81bf347eaba7f6941
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61287309"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

plannerRosterId := "plannerRoster-id"
graphClient.Planner().RostersById(&plannerRosterId).Delete(nil)


```