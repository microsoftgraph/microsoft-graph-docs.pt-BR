---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 3aa450b509b8537ac9fb6cc02474346ce7b6888a795995a3aa75ccba0050bec1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57271904"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PrivilegedRoleAssignmentCollectionPage privilegedRoleAssignments = graphClient.privilegedRoleAssignments()
    .buildRequest()
    .get();

```