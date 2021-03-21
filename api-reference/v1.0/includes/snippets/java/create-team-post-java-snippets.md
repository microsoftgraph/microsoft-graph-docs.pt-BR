---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b863d7b689f25ad3e81a75ef2c845a83eab8afa1
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50976343"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Team team = new Team();
team.additionalDataManager().put("template@odata.bind", new JsonPrimitive("https://graph.microsoft.com/v1.0/teamsTemplates('standard')"));
team.displayName = "My Sample Team";
team.description = "My Sample Team’s Description";

graphClient.teams()
    .buildRequest()
    .post(team);

```