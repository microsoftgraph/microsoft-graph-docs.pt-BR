---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 76b50651a377fa4ef9ca762da0f4662fea088c83
ms.sourcegitcommit: 64d27a0e3dcccc9d857e62aace4153e5d98fb3d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/03/2021
ms.locfileid: "60730540"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Content riskyUsers = graphClient.tenantRelationships().managedTenants().riskyUsers()
    .buildRequest()
    .get();

```