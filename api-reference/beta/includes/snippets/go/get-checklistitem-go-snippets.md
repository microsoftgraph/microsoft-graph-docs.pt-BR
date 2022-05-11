---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ed16847380e94e057492436f7bd84cda751d437c
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65324429"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

baseTaskListId := "baseTaskList-id"
baseTaskId := "baseTask-id"
checklistItemId := "checklistItem-id"
result, err := graphClient.Me().Tasks().ListsById(&baseTaskListId).TasksById(&baseTaskId).ChecklistItemsById(&checklistItemId).Get()


```