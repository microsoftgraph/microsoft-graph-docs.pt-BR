---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: c8fae4d5810c288618f2b24568d3087b5fb71497
ms.sourcegitcommit: 0bcc0a93f37db6013be40dc8d36717aeeeef7fb6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/16/2022
ms.locfileid: "63528049"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

ItemActivityStat itemActivityStat = graphClient.drives("{drive-id}").items("{item-id}").analytics().allTime()
    .buildRequest()
    .get();

```