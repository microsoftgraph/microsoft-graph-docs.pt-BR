---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 0718662666afe53d412cdfefe42147b3a4c34096
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/25/2021
ms.locfileid: "51208764"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Shift shift = graphClient.teams("{teamId}").schedule().shifts("{shiftId}")
    .buildRequest()
    .get();

```