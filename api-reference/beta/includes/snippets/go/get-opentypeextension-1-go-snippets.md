---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 44c3b7abf2e940335dc40304aae80201c24f7e55
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61034066"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

messageId := "message-id"
extensionId := "extension-id"
result, err := graphClient.Me().MessagesById(&messageId).ExtensionsById(&extensionId).Get(options)


```