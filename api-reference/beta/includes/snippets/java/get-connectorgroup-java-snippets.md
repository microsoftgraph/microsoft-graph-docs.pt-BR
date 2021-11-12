---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 86310b720552d12f4b64913fa0740be6cb360ed66e8781b68b184d063cf107e1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57326764"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ConnectorGroup connectorGroup = graphClient.onPremisesPublishingProfiles("applicationProxy").connectorGroups("{id}")
    .buildRequest()
    .get();

```