---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9718f72d430c7a18d22ebfd001b3623266fc16d2
ms.sourcegitcommit: 1d9193fa91f44d80ecdc2b82e37272df1c9630f6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/22/2022
ms.locfileid: "65629035"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Content tenantUsage = graphClient.tenantRelationships().managedTenants().tenantUsage()
    .buildRequest()
    .get();

```