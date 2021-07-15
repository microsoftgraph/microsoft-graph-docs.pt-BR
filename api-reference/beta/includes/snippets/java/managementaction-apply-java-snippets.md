---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f2a682c81550a9e4614263afc1dc1c4f363b5f6c
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/15/2021
ms.locfileid: "53442114"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String tenantId = "String";

String tenantGroupId = "String";

String managementTemplateId = "String";

graphClient.tenantRelationships().managedTenants().managementActions("{managementActionId}")
    .apply(ManagementActionApplyParameterSet
        .newBuilder()
        .withTenantId(tenantId)
        .withTenantGroupId(tenantGroupId)
        .withManagementTemplateId(managementTemplateId)
        .build())
    .buildRequest()
    .post();

```