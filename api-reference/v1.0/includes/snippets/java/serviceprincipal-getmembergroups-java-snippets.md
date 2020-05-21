---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e45b02538a463ec196ceefc7d26178c51ffc2ddf
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/21/2020
ms.locfileid: "44333990"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

boolean securityEnabledOnly = true;

graphClient.servicePrincipals("{id}")
    .getMemberGroups(securityEnabledOnly)
    .buildRequest()
    .post();

```