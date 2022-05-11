---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 900cb4bb9f262f3dd234291cfd971a34ada19652
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65324430"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

baseTaskListId := "baseTaskList-id"
baseTaskId := "baseTask-id"
checklistItemId := "checklistItem-id"
graphClient.Me().Tasks().ListsById(&baseTaskListId).TasksById(&baseTaskId).ChecklistItemsById(&checklistItemId).Delete()


```