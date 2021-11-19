---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 39f1e5aac828ade152935e0d68bead1ab3a3bbac
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61089705"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

plannerPlanId := "plannerPlan-id"
result, err := graphClient.Planner().PlansById(&plannerPlanId).Get(options)


```