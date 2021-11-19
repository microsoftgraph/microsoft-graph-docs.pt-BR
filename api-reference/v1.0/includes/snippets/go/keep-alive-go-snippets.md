---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 377bf9a53fb0df8a57f7e081e719536b16f40d0e
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2021
ms.locfileid: "61083128"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

callId := "call-id"
graphClient.Communications().CallsById(&callId).KeepAlive().Post(options)


```