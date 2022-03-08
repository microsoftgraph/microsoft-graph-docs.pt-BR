---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b0527903ac580aba26a168001dea9b8423a955a7
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2022
ms.locfileid: "63336568"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

CrossTenantAccessPolicy crossTenantAccessPolicy = graphClient.policies().crossTenantAccessPolicy()
    .buildRequest()
    .get();

```