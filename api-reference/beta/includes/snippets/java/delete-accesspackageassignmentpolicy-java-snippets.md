---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 322ab3d9638428344d5f1eaa4d1bba89f3afbe6b6003952d1f41ec3e3a1985d2
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57099867"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.identityGovernance().entitlementManagement().accessPackageAssignmentPolicies("{id}")
    .buildRequest()
    .delete();

```