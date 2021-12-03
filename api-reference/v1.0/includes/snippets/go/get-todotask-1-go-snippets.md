---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7435f9ebbe5a60906d0f7ad900c2ea671feaab17
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61286642"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

todoTaskListId := "todoTaskList-id"
todoTaskId := "todoTask-id"
result, err := graphClient.Me().Todo().ListsById(&todoTaskListId).TasksById(&todoTaskId).Get(nil)


```