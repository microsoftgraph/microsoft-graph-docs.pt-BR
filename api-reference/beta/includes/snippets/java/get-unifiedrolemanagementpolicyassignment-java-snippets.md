---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c88c8da18b6f8cacbfdfd8357cd50ee33af8e4a9de7c2a5bc78c222990429e70
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57102224"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UnifiedRoleManagementPolicyAssignment unifiedRoleManagementPolicyAssignment = graphClient.policies().roleManagementPolicyAssignments("d6e4112f-112f-d6e4-2f11-e4d62f11e4d6")
    .buildRequest()
    .get();

```