---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 5b0418e545a96a0e9b1af3ddcb20b29a0beef9205f8f37b76e0b05b885662ced
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57158225"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UnifiedRoleManagementPolicyCollectionPage roleManagementPolicies = graphClient.policies().roleManagementPolicies()
    .buildRequest()
    .get();

```