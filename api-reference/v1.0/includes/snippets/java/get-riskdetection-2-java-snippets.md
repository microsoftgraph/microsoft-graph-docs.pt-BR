---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: decf3f275ea5e5d4b1af905c1c9b249c4ecd255a
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62122030"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

RiskDetectionCollectionPage riskDetections = graphClient.identityProtection().riskDetections()
    .buildRequest()
    .get();

```