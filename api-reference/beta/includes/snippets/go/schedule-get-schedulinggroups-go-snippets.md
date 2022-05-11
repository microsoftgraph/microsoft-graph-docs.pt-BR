---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 59f9e384a2bac3d620d1d1f39b3f9e4c6937d142
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65325026"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

teamId := "team-id"
schedulingGroupId := "schedulingGroup-id"
result, err := graphClient.TeamsById(&teamId).Schedule().SchedulingGroupsById(&schedulingGroupId).Get()


```