---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e9e6a30e58876c5ccf23c3506b9df38a02b3bbed
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50955509"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

RiskDetectionCollectionPage riskDetections = graphClient.identityProtection().riskDetections()
    .buildRequest()
    .filter("riskEventType eq 'unfamiliarFeatures' or riskLevel eq 'medium'")
    .get();

```