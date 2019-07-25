---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 540eb2adc2e601456c1d1f8a293e2449c3830a6a
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/25/2019
ms.locfileid: "35878649"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IOnPremisesAgentCollectionPage agents = graphClient.onPremisesPublishingProfiles("provisioning").agents()
    .buildRequest()
    .expand("agentGroups")
    .get();

```