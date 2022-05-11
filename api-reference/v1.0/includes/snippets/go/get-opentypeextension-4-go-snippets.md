---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4eee142a0bc72ad4e261a25a076544dc821c30e2
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65324467"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

groupId := "group-id"
conversationThreadId := "conversationThread-id"
postId := "post-id"
extensionId := "extension-id"
result, err := graphClient.GroupsById(&groupId).ThreadsById(&conversationThreadId).PostsById(&postId).ExtensionsById(&extensionId).Get()


```