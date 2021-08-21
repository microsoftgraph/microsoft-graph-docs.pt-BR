---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 22474a07c04bbcd690a83a6cea95e4c33e909e80c584a87458fa5baf17707ded
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "56899094"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UnifiedRoleManagementPolicyAssignmentCollectionPage roleManagementPolicyAssignments = graphClient.policies().roleManagementPolicyAssignments()
    .buildRequest()
    .get();

```