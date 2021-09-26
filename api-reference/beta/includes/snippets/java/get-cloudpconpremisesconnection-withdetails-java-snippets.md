---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 2669314a1c63494eb88d3352c78da059a74c7fb62c36a4a2d700df18577c7e50
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "57100910"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

CloudPcOnPremisesConnection cloudPcOnPremisesConnection = graphClient.deviceManagement().virtualEndpoint().onPremisesConnections("{id}")
    .buildRequest()
    .select("id,displayName,healthCheckStatus,healthCheckStatusDetails,inUse")
    .get();

```