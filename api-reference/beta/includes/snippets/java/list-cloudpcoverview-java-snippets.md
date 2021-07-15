---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c4d00e6d9b8e43e31b5368ceaeee242c64073c50
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/15/2021
ms.locfileid: "53441472"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

CloudPcOverviewCollectionPage cloudPcsOverview = graphClient.tenantRelationships().managedTenants().cloudPcsOverview()
    .buildRequest()
    .get();

```