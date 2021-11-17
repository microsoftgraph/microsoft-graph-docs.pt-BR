---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 0d29a0c8a294b9e78406ca09db53a10c9be7e12667fd1d3f327ce950b1d8cc76
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57160313"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

AggregatedPolicyComplianceCollectionPage aggregatedPolicyCompliances = graphClient.tenantRelationships().managedTenants().aggregatedPolicyCompliances()
    .buildRequest()
    .get();

```