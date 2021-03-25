---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: df3babaf962545ad8408a396088d7efb19d06612
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/25/2021
ms.locfileid: "51211204"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ConnectorCollectionPage connectors = graphClient.onPremisesPublishingProfiles("applicationProxy").connectors()
    .buildRequest()
    .get();

```