---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9a2e95758a9cd86febde69febfc8dbe30514f46a
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61020282"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

chatId := "chat-id"
teamsAppInstallationId := "teamsAppInstallation-id"
graphClient.ChatsById(&chatId).InstalledAppsById(&teamsAppInstallationId).Upgrade().Post(options)


```