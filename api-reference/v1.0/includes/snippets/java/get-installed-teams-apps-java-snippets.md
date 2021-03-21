---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 79fce42ae1a071e5394ae026a4cef007c3a9f55f
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50968586"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TeamsAppInstallation teamsAppInstallation = graphClient.teams("{id}").installedApps("{id}")
    .buildRequest()
    .get();

```