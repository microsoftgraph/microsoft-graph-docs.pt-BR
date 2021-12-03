---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7bb36af99ed668d9b175ab9698e3db50840d026c
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61286864"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

todoTaskListId := "todoTaskList-id"
result, err := graphClient.Me().Todo().ListsById(&todoTaskListId).Get(nil)


```