---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f19919294166f1441916ce3b71a5e3615342c46d
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/09/2022
ms.locfileid: "63410926"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

baseTaskListId := "baseTaskList-id"
baseTaskId := "baseTask-id"
result, err := graphClient.Me().Tasks().ListsById(&baseTaskListId).TasksById(&baseTaskId).Delete(nil)


```