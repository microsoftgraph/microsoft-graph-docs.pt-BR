---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c9b0e7aeb97a708dbbd5d1bcdaca8fd6fbc0497a
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/15/2021
ms.locfileid: "53441109"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TenantGroup tenantGroup = graphClient.tenantRelationships().managedTenants().tenantGroups("{tenantGroupId}")
    .buildRequest()
    .get();

```