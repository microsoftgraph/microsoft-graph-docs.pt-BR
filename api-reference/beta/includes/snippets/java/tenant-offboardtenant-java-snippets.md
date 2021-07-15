---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 69ac24898ed6cee24e513df02d9f9f42eaf9ee16
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/15/2021
ms.locfileid: "53442492"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.tenantRelationships().managedTenants().tenants("{tenantId}")
    .offboardTenant()
    .buildRequest()
    .post();

```