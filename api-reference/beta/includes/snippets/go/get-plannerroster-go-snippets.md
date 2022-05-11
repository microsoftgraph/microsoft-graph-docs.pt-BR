---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 03e73976f44f7db936721e1e92fb1ab13fd6b5e5
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65323871"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

plannerRosterId := "plannerRoster-id"
result, err := graphClient.Planner().RostersById(&plannerRosterId).Get()


```