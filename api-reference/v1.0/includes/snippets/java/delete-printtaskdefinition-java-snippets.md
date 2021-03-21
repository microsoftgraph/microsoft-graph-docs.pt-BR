---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: ec5a5c5225451db79627cdd80c178a569add16d5
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50973943"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

graphClient.print().taskDefinitions("{printTaskDefinitionId}")
    .buildRequest()
    .delete();

```