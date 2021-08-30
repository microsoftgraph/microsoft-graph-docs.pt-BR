---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ca9787019a599362096df086f8d64a71c47406ea1fa0a44d0db431f769b4999d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57376583"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Team team = new Team();
team.additionalDataManager().put("template@odata.bind", new JsonPrimitive("https://graph.microsoft.com/beta/teamsTemplates('educationClass')"));
team.displayName = "My Class Team";
team.description = "My Class Team’s Description";

graphClient.teams()
    .buildRequest()
    .post(team);

```