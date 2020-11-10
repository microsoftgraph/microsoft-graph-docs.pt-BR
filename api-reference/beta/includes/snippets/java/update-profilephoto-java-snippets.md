---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: d2f197e007e0b1908b7b3f29bbebe288434c9ae4
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48981730"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

byte[] stream = Base64.getDecoder().decode("Binary data for the image");
    graphClient.me().photo().content()
    .buildRequest()
    .put(stream);

```