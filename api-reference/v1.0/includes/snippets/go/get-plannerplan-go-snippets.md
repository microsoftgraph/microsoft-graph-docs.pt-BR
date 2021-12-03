---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b0aa816fe18980c6f4ee2fd84062a29bd4533b74
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61286822"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

plannerPlanId := "plannerPlan-id"
result, err := graphClient.Planner().PlansById(&plannerPlanId).Get(nil)


```