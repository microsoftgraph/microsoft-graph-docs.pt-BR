---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a0e9cabb4e405b7bf65bf106dc803b01c0652c11a1ea9697e1bfbf77855c8020
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57214732"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PrivilegedRoleAssignmentCollectionPage privilegedRoleAssignments = graphClient.privilegedRoleAssignments()
    .buildRequest()
    .filter("isElevated eq true")
    .get();

```