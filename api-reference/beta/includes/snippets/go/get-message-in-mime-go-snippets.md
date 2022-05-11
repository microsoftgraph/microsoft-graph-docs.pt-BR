---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 68313fd50ee921906d0bfc901a5071786dff7eec
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65323698"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

messageId := "message-id"
graphClient.Me().MessagesById(&messageId).$value().Get()


```