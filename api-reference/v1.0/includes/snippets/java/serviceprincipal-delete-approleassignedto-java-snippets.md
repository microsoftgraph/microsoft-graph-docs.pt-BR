---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 0acdc4770c8f8ffbf6a696164f7e71b5e4d26c40
ms.sourcegitcommit: 503c72036c376a30e08c29df8e7730a7afcab66e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/10/2021
ms.locfileid: "52870560"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.servicePrincipals("{resource-SP-id}").appRoleAssignedTo("{principalId}")
    .buildRequest()
    .delete();

```