---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b27b42b86ac5539f75c8ff7cf064d95cdf1f84b0
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50969005"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Participant participant = graphClient.communications().calls("7531d31f-d10d-44de-802f-c569dbca451c").participants("7e1b4346-85a6-4bdd-abe3-d11c5d420efe")
    .buildRequest()
    .get();

```