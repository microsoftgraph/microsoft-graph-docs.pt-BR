---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d07b6ac54e9a0610c841b0c89371aa25c442d5cc435b470c9deff86a07c01346
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57273018"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ManagementIntent managementIntent = graphClient.tenantRelationships().managedTenants().managementIntents("{managementIntentId}")
    .buildRequest()
    .get();

```