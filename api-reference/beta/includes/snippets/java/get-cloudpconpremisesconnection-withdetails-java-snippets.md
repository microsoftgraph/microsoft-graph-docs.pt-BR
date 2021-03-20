---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 33c27269e5aa2cfa2d8141b076ae7e210205d887
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50967197"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

CloudPcOnPremisesConnection cloudPcOnPremisesConnection = graphClient.deviceManagement().virtualEndpoint().onPremisesConnections("{id}")
    .buildRequest()
    .select("id,displayName,healthCheckStatus,healthCheckStatusDetails,inUse")
    .get();

```