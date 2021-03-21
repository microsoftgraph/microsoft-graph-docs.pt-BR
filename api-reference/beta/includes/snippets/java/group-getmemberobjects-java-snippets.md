---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e9fefdf18e7284751fa3e1eeb671e8e6b6c27c97
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50982088"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Boolean securityEnabledOnly = false;

graphClient.groups("{id}")
    .getMemberObjects(DirectoryObjectGetMemberObjectsParameterSet
        .newBuilder()
        .withSecurityEnabledOnly(securityEnabledOnly)
        .build())
    .buildRequest()
    .post();

```