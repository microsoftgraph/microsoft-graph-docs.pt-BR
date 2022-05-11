---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 71c6f333aff4330265eacdd99e7c4c7dcc6f40f6
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65322902"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

chatId := "chat-id"
result, err := graphClient.ChatsById(&chatId).PermissionGrants().Get()


```