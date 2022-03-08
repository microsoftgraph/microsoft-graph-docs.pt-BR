---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b4e816021f4b476799454366199b1e2634b0acdb
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2022
ms.locfileid: "63336631"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

CrossTenantAccessPolicy crossTenantAccessPolicy = new CrossTenantAccessPolicy();
crossTenantAccessPolicy.displayName = "CrossTenantAccessPolicy";

graphClient.policies().crossTenantAccessPolicy()
    .buildRequest()
    .patch(crossTenantAccessPolicy);

```