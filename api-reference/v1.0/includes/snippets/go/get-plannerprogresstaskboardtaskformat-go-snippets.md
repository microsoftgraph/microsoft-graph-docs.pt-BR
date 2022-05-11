---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4234cb15afc5973f4bb9e2a09723d4ef5bc5f9fd
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65322415"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

plannerTaskId := "plannerTask-id"
result, err := graphClient.Planner().TasksById(&plannerTaskId).ProgressTaskBoardFormat().Get()


```