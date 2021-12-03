---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d05b705d4f12823c9ebf35f9c6181d658937183e
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61287283"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

groupId := "group-id"
conversationId := "conversation-id"
result, err := graphClient.GroupsById(&groupId).ConversationsById(&conversationId).Threads().Get(nil)


```