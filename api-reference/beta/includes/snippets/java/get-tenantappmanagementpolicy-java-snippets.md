---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a8345ca66ffd548462c92b8b7dd479cf7fab1d34
ms.sourcegitcommit: 9b8abc940a68dac6ee5da105ca29800cb59775f6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/25/2021
ms.locfileid: "58514092"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TenantAppManagementPolicy tenantAppManagementPolicy = graphClient.policies().defaultAppManagementPolicy()
    .buildRequest()
    .get();

```