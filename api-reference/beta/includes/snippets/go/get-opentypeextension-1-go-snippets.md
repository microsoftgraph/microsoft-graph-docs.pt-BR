---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 31904de272e3f8ab384794efae406984de24d26e
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61287216"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

messageId := "message-id"
extensionId := "extension-id"
result, err := graphClient.Me().MessagesById(&messageId).ExtensionsById(&extensionId).Get(nil)


```