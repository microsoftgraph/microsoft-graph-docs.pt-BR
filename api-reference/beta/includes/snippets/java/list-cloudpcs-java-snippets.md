---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 37f665257d316a4f0e1fb5422323eb678928df62
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/01/2020
ms.locfileid: "49522304"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ICloudPCCollectionPage cloudPCs = graphClient.deviceManagement().virtualEndpoint().cloudPCs()
    .buildRequest()
    .get();

```