---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a48be0078e7a6be959b65d71ea8bcdfe881e5c953fc5191e522fe0f9fe4b4f35
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57100960"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Approval approval = graphClient.identityGovernance().entitlementManagement().accessPackageAssignmentApprovals("abd306ef-f7b2-4a10-9fd1-493454322489")
    .buildRequest()
    .get();

```