---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 544b981cb6144eb6009e412af4be560aab309d31
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2022
ms.locfileid: "63335749"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

CrossTenantAccessPolicyConfigurationPartner crossTenantAccessPolicyConfigurationPartner = graphClient.policies().crossTenantAccessPolicy().partners("9c5d131d-b1c3-4fc4-9e3f-c6557947d551")
    .buildRequest()
    .get();

```