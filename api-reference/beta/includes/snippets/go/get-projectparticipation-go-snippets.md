---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: be5d6c32afdd3a99336a3708dd23699f2a645dab
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65324112"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

projectParticipationId := "projectParticipation-id"
result, err := graphClient.Me().Profile().ProjectsById(&projectParticipationId).Get()


```