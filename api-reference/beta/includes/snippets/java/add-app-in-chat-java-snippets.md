---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 17567965650880b208ed05419209965c57a74b84
ms.sourcegitcommit: 75428fc7535662f34e965c6b69fef3a53fdaf1cb
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/16/2020
ms.locfileid: "49689764"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TeamsAppInstallation teamsAppInstallation = new TeamsAppInstallation();
teamsAppInstallation.additionalDataManager().put("teamsApp@odata.bind", new JsonPrimitive("https://graph.microsoft.com/beta/appCatalogs/teamsApps/12345678-9abc-def0-123456789a"));

graphClient.chats("19:ea28e88c00e94c7786b065394a61f296@thread.v2").installedApps()
    .buildRequest()
    .post(teamsAppInstallation);

```