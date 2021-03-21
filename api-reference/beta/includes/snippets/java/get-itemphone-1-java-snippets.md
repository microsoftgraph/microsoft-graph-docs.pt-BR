---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: bb17993fb7e2d8c8ee733d5714a79fce5737117c
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50954523"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ItemPhone itemPhone = graphClient.me().profile().phones("{id}")
    .buildRequest()
    .get();

```