---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e90fa0eb9044a7108965a7864f201d268fbb3bdc
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65324116"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

userId := "user-id"
result, err := graphClient.UsersById(&userId).Planner().RosterPlans().Get()


```