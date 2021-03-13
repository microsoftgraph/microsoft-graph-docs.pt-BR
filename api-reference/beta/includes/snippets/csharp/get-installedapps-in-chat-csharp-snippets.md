---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8e4a5ebbb77124dd0b088aa2e69e182024f9875f
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50775847"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var teamsAppInstallation = await graphClient.Chats["{chat-id}"].InstalledApps["{teamsAppInstallation-id}"]
    .Request()
    .GetAsync();

```