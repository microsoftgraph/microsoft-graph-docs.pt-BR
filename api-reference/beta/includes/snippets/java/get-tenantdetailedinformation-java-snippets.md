---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d2ec787c361f896ac08ea42580509a009c52e6b6
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/15/2021
ms.locfileid: "53441795"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TenantDetailedInformation tenantDetailedInformation = graphClient.tenantRelationships().managedTenants().tenantsDetailedInformation("{tenantDetailedInformationId}")
    .buildRequest()
    .get();

```