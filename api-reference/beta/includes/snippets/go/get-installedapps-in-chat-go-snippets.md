---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2005e31e17b07a2382995942dc04e4a5cb68b0c0
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2022
ms.locfileid: "65324153"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

chatId := "chat-id"
teamsAppInstallationId := "teamsAppInstallation-id"
result, err := graphClient.ChatsById(&chatId).InstalledAppsById(&teamsAppInstallationId).Get()


```