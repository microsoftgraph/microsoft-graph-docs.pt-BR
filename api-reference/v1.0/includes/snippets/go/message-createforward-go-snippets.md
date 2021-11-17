---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: dd963ce4481d5a1610050af892e3fab831cfe90f
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "60996193"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

messageId := "message-id"
result, err := graphClient.Me().MessagesById(&messageId).CreateForward().Post(options)


```