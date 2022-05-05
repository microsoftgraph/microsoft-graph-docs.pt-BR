---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 8686a1bde1162bc86107e54279ce9c86d6ab39c1
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/05/2022
ms.locfileid: "65203603"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

SimulationAutomationCollectionPage simulationAutomations = graphClient.security().attackSimulation().simulationAutomations()
    .buildRequest()
    .get();

```