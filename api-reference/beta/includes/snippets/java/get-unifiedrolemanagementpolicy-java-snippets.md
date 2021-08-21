---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 7cbee167a7b689a95196899b1fe91929839f30846f25f6d3e1acc1b7a693a8fa
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57272644"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UnifiedRoleManagementPolicy unifiedRoleManagementPolicy = graphClient.policies().roleManagementPolicies("f93a5c37-5c37-f93a-375c-3af9375c3af9")
    .buildRequest()
    .get();

```