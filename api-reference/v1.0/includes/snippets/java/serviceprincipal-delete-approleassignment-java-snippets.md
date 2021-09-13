---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 51959a1c56e1adc33ddd99c9b092efdebf65829f17be03da3fb4075643220e8b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57330009"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.servicePrincipals("{servicePrincipal-id}").appRoleAssignments("{appRoleAssignment-id}")
    .buildRequest()
    .delete();

```