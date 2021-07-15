---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 3b4931fd608b7d0c5816f3765098bc5c09171103
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/15/2021
ms.locfileid: "53442715"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TenantTag tenantTag = new TenantTag();
tenantTag.displayName = "Onboarding";
tenantTag.description = "Tenants that we are currently onboarding";

graphClient.tenantRelationships().managedTenants().tenantTags("{tenantTagId}")
    .buildRequest()
    .patch(tenantTag);

```