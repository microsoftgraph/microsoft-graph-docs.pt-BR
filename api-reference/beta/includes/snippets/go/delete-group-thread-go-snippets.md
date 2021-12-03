---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 69e86cd1c0df64f1df0191365b252fdf481d2403
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61286813"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

groupId := "group-id"
conversationThreadId := "conversationThread-id"
graphClient.GroupsById(&groupId).ThreadsById(&conversationThreadId).Delete(nil)


```