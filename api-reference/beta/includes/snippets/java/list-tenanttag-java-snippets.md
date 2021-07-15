---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c96108f78cccfd5569d71e364a0427f6501bf948
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/15/2021
ms.locfileid: "53442358"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TenantTagCollectionPage tenantTags = graphClient.tenantRelationships().managedTenants().tenantTags()
    .buildRequest()
    .get();

```