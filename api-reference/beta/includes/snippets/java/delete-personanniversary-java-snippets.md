---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 6f3914ccfb976cac9cf53245007e819609313a53
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50974015"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.me().profile().anniversaries("{id}")
    .buildRequest()
    .delete();

```