---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e48d5d672aa8c94e5efbea4a58ae9b6c6126e151
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/15/2021
ms.locfileid: "53443001"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ManagementIntentCollectionPage managementIntents = graphClient.tenantRelationships().managedTenants().managementIntents()
    .buildRequest()
    .get();

```