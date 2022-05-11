---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fd6c4e7b25d3ec3a6835d54882e6ae2dba3efd37
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65324052"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

simulationAutomationId := "simulationAutomation-id"
result, err := graphClient.Security().AttackSimulation().SimulationAutomationsById(&simulationAutomationId).Runs().Get()


```