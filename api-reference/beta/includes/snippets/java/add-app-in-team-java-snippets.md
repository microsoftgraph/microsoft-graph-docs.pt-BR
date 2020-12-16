---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: de9781060cbbed5bc54ba0e3efc2f5c348ddfde7
ms.sourcegitcommit: 75428fc7535662f34e965c6b69fef3a53fdaf1cb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/16/2020
ms.locfileid: "49690313"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TeamsAppInstallation teamsAppInstallation = new TeamsAppInstallation();
teamsAppInstallation.additionalDataManager().put("teamsApp@odata.bind", new JsonPrimitive("https://graph.microsoft.com/beta/appCatalogs/teamsApps/12345678-9abc-def0-123456789a"));

graphClient.teams("87654321-0abc-zqf0-321456789q").installedApps()
    .buildRequest()
    .post(teamsAppInstallation);

```