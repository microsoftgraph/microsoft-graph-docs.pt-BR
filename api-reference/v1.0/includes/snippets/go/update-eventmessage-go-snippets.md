---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 156bc1da5650b9d7855d8f43f33f9a5a384ee541
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61025426"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

messageId := "message-id"
graphClient.Me().MessagesById(&messageId).Patch(options)


```