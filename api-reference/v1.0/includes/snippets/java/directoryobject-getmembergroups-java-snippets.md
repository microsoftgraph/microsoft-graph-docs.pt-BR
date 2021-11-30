---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 4956430abc3ec33fb7f499a3b497cf1a2d845fe9
ms.sourcegitcommit: e497ed9bb56400bdd2bb53d52ddf057d9966220b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/30/2021
ms.locfileid: "61224093"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Boolean securityEnabledOnly = false;

graphClient.directoryObjects("0049d944-a805-4680-9f54-3ab292090309")
    .getMemberGroups(DirectoryObjectGetMemberGroupsParameterSet
        .newBuilder()
        .withSecurityEnabledOnly(securityEnabledOnly)
        .build())
    .buildRequest()
    .post();

```