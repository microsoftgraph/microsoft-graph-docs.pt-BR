---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c530e8a29b59eb3afe38f8c69c78e7ac4ad75afe
ms.sourcegitcommit: 75428fc7535662f34e965c6b69fef3a53fdaf1cb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/16/2020
ms.locfileid: "49691293"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IUserScopeTeamsAppInstallationCollectionPage installedApps = graphClient.users("{id}").teamwork().installedApps()
    .buildRequest()
    .expand("teamsAppDefinition")
    .get();

```