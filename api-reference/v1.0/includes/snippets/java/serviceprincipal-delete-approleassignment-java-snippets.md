---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c5e2576bc15ca89f8eb0b14432d60ed91d7be7c3
ms.sourcegitcommit: 503c72036c376a30e08c29df8e7730a7afcab66e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/10/2021
ms.locfileid: "52870511"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.servicePrincipals("{servicePrincipal-id}").appRoleAssignments("{appRoleAssignment-id}")
    .buildRequest()
    .delete();

```