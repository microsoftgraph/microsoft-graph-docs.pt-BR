---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2f5743cc13e7e37a65edeb910c64992b2c33034e
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65323720"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
user := msgraphsdk.NewTeamworkUserIdentity()
requestBody.SetUser(user)
id := "d864e79f-a516-4d0f-9fee-0eeb4d61fdc2"
user.SetId(&id)
tenantId := "2a690434-97d9-4eed-83a6-f5f13600199a"
requestBody.SetTenantId(&tenantId)
chatId := "chat-id"
graphClient.ChatsById(&chatId).HideForUser(chat-id).Post(requestBody)


```