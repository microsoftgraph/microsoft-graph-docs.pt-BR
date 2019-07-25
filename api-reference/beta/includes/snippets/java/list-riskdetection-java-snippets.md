---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8cbae92a89363773fe4943ab13792df39ba26952
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35871097"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IRiskDetectionCollectionPage riskDetections = graphClient.riskDetections()
    .buildRequest()
    .get();

```