---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 69ebe20dcc3769a41c70fb815f77490091ac8f7a
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/15/2021
ms.locfileid: "53441930"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ManagementActionTenantDeploymentStatusCollectionPage managementActionTenantDeploymentStatuses = graphClient.tenantRelationships().managedTenants().managementActionTenantDeploymentStatuses()
    .buildRequest()
    .get();

```