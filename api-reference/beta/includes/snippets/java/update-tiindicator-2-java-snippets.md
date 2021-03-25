---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: b5cbab6b3ad7a6cbd9c844263353d2a40c3b0977
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/25/2021
ms.locfileid: "51210124"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

LinkedList<Option> requestOptions = new LinkedList<Option>();
requestOptions.add(new HeaderOption("Prefer", "return=representation"));

TiIndicator tiIndicator = new TiIndicator();
tiIndicator.additionalInformation = "additionalInformation-after-update";
tiIndicator.confidence = 42;
tiIndicator.description = "description-after-update";

graphClient.security().tiIndicators("{id}")
    .buildRequest( requestOptions )
    .patch(tiIndicator);

```