---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b0e0ceef9260907133cce64b0f1d102b6b91aa73
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2022
ms.locfileid: "63334818"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ServicePrincipalRiskDetectionCollectionPage servicePrincipalRiskDetections = graphClient.identityProtection().servicePrincipalRiskDetections()
    .buildRequest()
    .filter("riskEventType eq 'investigationsThreatIntelligence' or riskLevel eq 'medium'")
    .get();

```