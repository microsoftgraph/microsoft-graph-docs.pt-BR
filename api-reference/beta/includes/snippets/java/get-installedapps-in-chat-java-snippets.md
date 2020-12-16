---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 23bfb0e0416bc2a71a54ee1b59e8bdf271e8a5bd
ms.sourcegitcommit: 75428fc7535662f34e965c6b69fef3a53fdaf1cb
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/16/2020
ms.locfileid: "49690022"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TeamsAppInstallation teamsAppInstallation = graphClient.chats("19:d65713bc498c4a428c71ef9353e6ce20@thread.v2").installedApps("MTk6ZDY1NzEzYmM0OThjNGE0MjhjNzFlZjkzNTNlNmNlMjBAdGhyZWFkLnYyIyMwMDAwMTAxNi1kZTA1LTQ5MmUtOTEwNi00ODI4ZmM4YTg2ODc=")
    .buildRequest()
    .get();

```