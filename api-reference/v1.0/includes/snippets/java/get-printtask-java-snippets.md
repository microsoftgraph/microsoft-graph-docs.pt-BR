---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: f6069c9b23d4e785e9275774015fee563c1430f8
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50978631"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PrintTask printTask = graphClient.print().taskDefinitions("{taskDefinitionId}").tasks("{taskId}")
    .buildRequest()
    .get();

```