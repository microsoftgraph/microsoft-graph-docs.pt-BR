---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 82ba895eaf7a061c7f6dabf7bf9198cdccf54463
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/09/2022
ms.locfileid: "63411101"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

messageId := "message-id"
extensionId := "extension-id"
result, err := graphClient.Me().MessagesById(&messageId).ExtensionsById(&extensionId).Delete(nil)


```