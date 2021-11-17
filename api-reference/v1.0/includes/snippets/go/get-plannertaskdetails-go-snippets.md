---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ee785cbad90a1b293e84cf20f17af25e38167033
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61023067"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

plannerTaskId := "plannerTask-id"
result, err := graphClient.Planner().TasksById(&plannerTaskId).Details().Get(options)


```