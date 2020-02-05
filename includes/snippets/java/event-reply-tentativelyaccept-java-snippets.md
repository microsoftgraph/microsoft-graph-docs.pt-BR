---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 3e8218c90f07e358af83c4136c8e69b604672eb6
ms.sourcegitcommit: 7b286637aa332cfd534a41526950b4f6272e0fd7
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/05/2020
ms.locfileid: "41774617"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String comment = "I will probably be able to make it.";

boolean sendResponse = true;

graphClient.me().events("AAMkADADVj3fyAABZ5ieyAAA=")
    .tentativelyAccept(sendResponse,comment)
    .buildRequest()
    .post();

```