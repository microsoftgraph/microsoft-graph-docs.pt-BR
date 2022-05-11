---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c8dc7eb6e7f4ca9f4b6415294a3031ffc8000a0b
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65324506"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

plannerRosterId := "plannerRoster-id"
graphClient.Planner().RostersById(&plannerRosterId).Delete()


```