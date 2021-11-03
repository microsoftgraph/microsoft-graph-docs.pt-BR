---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c0028ef0c7cdfe9af6236ab3654b22f97a4a933f
ms.sourcegitcommit: 64d27a0e3dcccc9d857e62aace4153e5d98fb3d0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/03/2021
ms.locfileid: "60730505"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Content response = graphClient.tenantRelationships().managedTenants().riskyUsers().{riskyUserId}()
    .buildRequest()
    .get();

```