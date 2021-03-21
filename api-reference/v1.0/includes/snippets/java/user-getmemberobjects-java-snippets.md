---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 335d48ad45f020f48d9cdede2dce8ee35c362640
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50982785"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Boolean securityEnabledOnly = true;

graphClient.me()
    .getMemberObjects(DirectoryObjectGetMemberObjectsParameterSet
        .newBuilder()
        .withSecurityEnabledOnly(securityEnabledOnly)
        .build())
    .buildRequest()
    .post();

```