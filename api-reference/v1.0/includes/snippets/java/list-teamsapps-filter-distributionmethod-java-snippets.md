---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f9a200a25e2a6e986d88d89ec018b526eaa7fed6
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50968552"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TeamsAppCollectionPage teamsApps = graphClient.appCatalogs().teamsApps()
    .buildRequest()
    .filter("distributionMethod eq 'organization'")
    .get();

```