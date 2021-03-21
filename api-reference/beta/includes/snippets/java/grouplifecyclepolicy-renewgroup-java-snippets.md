---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 19755933229ed8c93ae9608483eb36a6ca59d4a9
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50978087"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String groupId = "ffffffff-ffff-ffff-ffff-ffffffffffff";

graphClient.groupLifecyclePolicies()
    .renewGroup(GroupLifecyclePolicyRenewGroupParameterSet
        .newBuilder()
        .withGroupId(groupId)
        .build())
    .buildRequest()
    .post();

```