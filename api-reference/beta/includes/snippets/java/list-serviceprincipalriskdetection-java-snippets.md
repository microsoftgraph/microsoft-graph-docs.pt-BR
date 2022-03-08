---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9cdb14dde2925704fb46e809360830d2d64824ce
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2022
ms.locfileid: "63334790"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ServicePrincipalRiskDetectionCollectionPage servicePrincipalRiskDetections = graphClient.identityProtection().servicePrincipalRiskDetections()
    .buildRequest()
    .get();

```