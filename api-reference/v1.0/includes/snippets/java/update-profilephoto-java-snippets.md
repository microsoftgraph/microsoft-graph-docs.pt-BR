---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c04c1e25231b5c67c946c6731e10980107f21cdb
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50980998"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

byte[] stream = Base64.getDecoder().decode("Binary data for the image");
    graphClient.me().photo().content()
    .buildRequest()
    .put(stream);

```