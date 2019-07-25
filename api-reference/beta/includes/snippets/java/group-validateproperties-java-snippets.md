---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 213ce90d6913c9fcdfd2c429441099d04a4e1a61
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35857727"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String displayName = "Myprefix_test_mysuffix";

String mailNickname = "Myprefix_test_mysuffix";

String onBehalfOfUserId = "onBehalfOfUserId-value";

graphClient.groups("{id}")
    .validateProperties(displayName,mailNickname,onBehalfOfUserId)
    .buildRequest()
    .post();

```