---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c1be2243fb707d5a81a0c5b77b0d8801c3dfac58
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48957356"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IConnectorGroupCollectionPage connectorGroups = graphClient.onPremisesPublishingProfiles("applicationProxy").connectorGroups()
    .buildRequest()
    .get();

```