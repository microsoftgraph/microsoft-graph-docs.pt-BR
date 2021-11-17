---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d52ba02bc12512aa6bafe27e6b14da9e32670e090f90eae645fa8a7db14494ea
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57213703"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TenantCustomizedInformation tenantCustomizedInformation = graphClient.tenantRelationships().managedTenants().tenantsCustomizedInformation("{tenantCustomizedInformationId}")
    .buildRequest()
    .get();

```