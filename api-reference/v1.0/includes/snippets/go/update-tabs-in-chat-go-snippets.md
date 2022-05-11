---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5258bf1ec33892f5c7f934f490889d7da7fd3df0
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65325644"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewTeamsTab()
displayName := "My Contoso Tab - updated again"
requestBody.SetDisplayName(&displayName)
chatId := "chat-id"
teamsTabId := "teamsTab-id"
graphClient.ChatsById(&chatId).TabsById(&teamsTabId).Patch(requestBody)


```