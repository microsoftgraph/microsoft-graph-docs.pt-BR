---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: cc7b66a41234ffedaa8c6419d90c8cc52edddb71
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/25/2021
ms.locfileid: "51210453"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.deviceManagement().virtualEndpoint().onPremisesConnections("{id}")
    .runHealthChecks()
    .buildRequest()
    .post();

```