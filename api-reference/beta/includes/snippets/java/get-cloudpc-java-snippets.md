---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a3dca78569f04d16aab2cbcc15e5b8ee4df850a6
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/01/2020
ms.locfileid: "49521947"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

CloudPC cloudPC = graphClient.deviceManagement().virtualEndpoint().cloudPCs("{id}")
    .buildRequest()
    .get();

```