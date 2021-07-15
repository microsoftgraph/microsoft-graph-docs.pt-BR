---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ed92e10cb82d11c539777223bd517fac27d69caf
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/15/2021
ms.locfileid: "53442595"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ManagementActionTenantDeploymentStatus managementActionTenantDeploymentStatus = graphClient.tenantRelationships().managedTenants().managementActionTenantDeploymentStatuses("{managementActionTenantDeploymentStatusId}")
    .buildRequest()
    .get();

```