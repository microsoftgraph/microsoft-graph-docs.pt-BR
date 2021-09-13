---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a0a71e732a0dd5ac0405bbe3abeee4e64a17c9b8bd15cf90084b5b5ac76151f3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56899958"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String displayName = "Myprefix_test_mysuffix";

String mailNickname = "Myprefix_test_mysuffix";

UUID onBehalfOfUserId = UUID.fromString("onBehalfOfUserId-value");

graphClient.groups("{id}")
    .validateProperties(GroupValidatePropertiesParameterSet
        .newBuilder()
        .withDisplayName(displayName)
        .withMailNickname(mailNickname)
        .withOnBehalfOfUserId(onBehalfOfUserId)
        .build())
    .buildRequest()
    .post();

```