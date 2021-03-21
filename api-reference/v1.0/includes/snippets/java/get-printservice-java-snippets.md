---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: a945b6c978fc60bbe93925d7d8947bde2f80de61
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50969486"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

PrintService printService = graphClient.print().services("{printServiceId}")
    .buildRequest()
    .get();

```