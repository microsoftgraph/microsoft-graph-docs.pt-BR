---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9972f61493567bbfd2b52e07711f1ce21183d392
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2022
ms.locfileid: "63336519"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

CrossTenantAccessPolicyConfigurationPartnerCollectionPage partners = graphClient.policies().crossTenantAccessPolicy().partners()
    .buildRequest()
    .get();

```