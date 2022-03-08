---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 323db6012991954a6d05fec0ef2c7dadfa2204b4
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2022
ms.locfileid: "63337289"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ServicePrincipalRiskDetection servicePrincipalRiskDetection = graphClient.identityProtection().servicePrincipalRiskDetections("{servicePrincipalRiskDetectionId}")
    .buildRequest()
    .get();

```