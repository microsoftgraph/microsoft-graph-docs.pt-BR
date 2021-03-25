---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a2ff7f6bb2f13fbd4e0fc1360b04d716e49f7141
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/25/2021
ms.locfileid: "51211027"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ConnectorGroup connectorGroup = new ConnectorGroup();
connectorGroup.name = "name-value";
connectorGroup.region = ConnectorGroupRegion.NAM;

graphClient.onPremisesPublishingProfiles("applicationProxy").connectorGroups("{id}")
    .buildRequest()
    .patch(connectorGroup);

```