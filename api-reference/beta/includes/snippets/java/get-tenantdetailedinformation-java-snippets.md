---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 97cf85aba26284023201e3fd8c7f0e6641a99a814d7d6e120f700c8ea701a0e4
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57213791"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TenantDetailedInformation tenantDetailedInformation = graphClient.tenantRelationships().managedTenants().tenantsDetailedInformation("{tenantDetailedInformationId}")
    .buildRequest()
    .get();

```