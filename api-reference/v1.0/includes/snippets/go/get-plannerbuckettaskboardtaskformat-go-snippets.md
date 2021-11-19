---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6f9dbe1f0d6d25fe4c7c2fbcee1dd068fc113f5b
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61099138"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

plannerTaskId := "plannerTask-id"
result, err := graphClient.Planner().TasksById(&plannerTaskId).BucketTaskBoardFormat().Get(options)


```