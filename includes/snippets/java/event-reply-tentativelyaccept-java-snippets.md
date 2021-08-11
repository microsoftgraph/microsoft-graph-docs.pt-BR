---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: fcb947ce881cb8c7aeec7cffb3a0278e5dae2dd5931cc1f4db22f8bf500cb4fc
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54129723"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

String comment = "I will probably be able to make it.";

boolean sendResponse = true;

graphClient.me().events("AAMkADADVj3fyAABZ5ieyAAA=")
    .tentativelyAccept(comment,sendResponse)
    .buildRequest()
    .post();

```