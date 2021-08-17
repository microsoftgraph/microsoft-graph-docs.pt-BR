---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 9585993d5775d2ee2c7bd31938735580e49e34ed
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58259097"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ServiceHealthCollectionPage healthOverviews = graphClient.admin().serviceAnnouncement().healthOverviews()
    .buildRequest()
    .expand("issues")
    .get();

```