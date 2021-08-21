---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 52826dd7ea29df3897af17041977ea2c3435d47b320055107ecc98a395097bf3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57272287"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PrivilegedRoleAssignmentRequestCollectionPage privilegedRoleAssignmentRequests = graphClient.privilegedRoleAssignmentRequests()
    .buildRequest()
    .get();

```