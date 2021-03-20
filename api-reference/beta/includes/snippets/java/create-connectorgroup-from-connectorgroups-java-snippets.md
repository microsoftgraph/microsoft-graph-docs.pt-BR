---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: e407d4a0f2d808a3df987d0cdc04fb428952aeb2
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50969309"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ConnectorGroup connectorGroup = new ConnectorGroup();
connectorGroup.name = "name-value";
connectorGroup.isDefault = false;

graphClient.onPremisesPublishingProfiles("applicationProxy").connectorGroups()
    .buildRequest()
    .post(connectorGroup);

```