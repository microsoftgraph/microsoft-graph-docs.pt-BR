---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8023ce56d555f7545c9a933ad8a078bfe24386fe
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50941462"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ThreatAssessmentRequest threatAssessmentRequest = graphClient.informationProtection().threatAssessmentRequests("49c5ef5b-1f65-444a-e6b9-08d772ea2059")
    .buildRequest()
    .get();

```