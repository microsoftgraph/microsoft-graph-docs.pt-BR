---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 09fb101b9fac75eb1b413e849f23dd6145105301
ms.sourcegitcommit: 36bae3615df41876493b25da478e589d1974f97b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/29/2021
ms.locfileid: "59995363"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

SimulationReportOverview simulationReportOverview = graphClient.customRequest("/security/attackSimulation/simulations/{id}/report/overview", SimulationReportOverview.class)
    .buildRequest()
    .get();

```