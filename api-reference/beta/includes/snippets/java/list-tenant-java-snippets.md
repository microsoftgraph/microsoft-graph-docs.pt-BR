---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a5ad871a16b599aea69ad3cfe6da6b600bfe3199d58c0c653ffc52ebcfae6626
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56899950"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TenantCollectionPage tenants = graphClient.tenantRelationships().managedTenants().tenants()
    .buildRequest()
    .get();

```