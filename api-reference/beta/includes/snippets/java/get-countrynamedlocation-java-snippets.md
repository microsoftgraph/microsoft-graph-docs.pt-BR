---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 391fd247c3177b033b5bd21993a75ea9d9960213
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50979987"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

NamedLocation namedLocation = graphClient.identity().conditionalAccess().namedLocations("1c4427fd-0885-4a3d-8b23-09a899ffa959")
    .buildRequest()
    .get();

```