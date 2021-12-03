---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ae8639c1d331c97d361e35770e7efdb15bb68b40
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/03/2021
ms.locfileid: "61285921"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

messageId := "message-id"
extensionId := "extension-id"
graphClient.Me().MessagesById(&messageId).ExtensionsById(&extensionId).Delete(nil)


```