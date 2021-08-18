---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6e37df31a05488ec16600d4bff024ac0788908f6a015256478df0edc770db4cc
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57216034"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

OnlineMeeting onlineMeeting = new OnlineMeeting();
LobbyBypassSettings lobbyBypassSettings = new LobbyBypassSettings();
lobbyBypassSettings.isDialInBypassEnabled = true;
onlineMeeting.lobbyBypassSettings = lobbyBypassSettings;

graphClient.me().onlineMeetings("MSpkYzE3Njc0Yy04MWQ5LTRhZGItYmZi")
    .buildRequest()
    .patch(onlineMeeting);

```