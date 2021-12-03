---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 3f131903ce0770f9379034bfa5bd1cc7e7694bec
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61286736"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

groupId := "group-id"
conversationThreadId := "conversationThread-id"
postId := "post-id"
result, err := graphClient.GroupsById(&groupId).ThreadsById(&conversationThreadId).PostsById(&postId).Get(nil)


```