---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9c728901f9ef0047c8a49d4c426b2a2003eef4df
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/09/2022
ms.locfileid: "63411385"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

chatId := "chat-id"
teamsAppInstallationId := "teamsAppInstallation-id"
result, err := graphClient.ChatsById(&chatId).InstalledAppsById(&teamsAppInstallationId).Delete(nil)


```