---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f9e049241d78751748f4c80293cbc0b6f9202594
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/25/2021
ms.locfileid: "51209146"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

TodoTaskList todoTaskList = graphClient.me().todo().lists("AAMkADIyAAAAABrJAAA=")
    .buildRequest()
    .get();

```