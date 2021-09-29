---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 472ead3753692cc588e8b685cd8338964c36d042
ms.sourcegitcommit: 36bae3615df41876493b25da478e589d1974f97b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/29/2021
ms.locfileid: "59995968"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

SimulationCollectionPage simulations = graphClient.security().attackSimulation().simulations()
    .buildRequest()
    .get();

```