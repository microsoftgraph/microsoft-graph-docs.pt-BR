---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 12f83828a55afdbdbea8daa7867ea351c66a8fc3
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/15/2021
ms.locfileid: "53441798"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String tenantId = "String";

graphClient.tenantRelationships().managedTenants().tenantGroups()
    .tenantSearch(TenantGroupTenantSearchParameterSet
        .newBuilder()
        .withTenantId(tenantId)
        .build())
    .buildRequest()
    .post();

```