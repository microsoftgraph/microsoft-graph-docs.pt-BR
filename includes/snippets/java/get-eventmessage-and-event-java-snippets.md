---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 573615474f59d67ec0be11281a488949988e4cf2
ms.sourcegitcommit: 7b286637aa332cfd534a41526950b4f6272e0fd7
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/05/2020
ms.locfileid: "41774611"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Message message = graphClient.me().messages("AAMkADADVj3fyAABZ5hYdAAA=")
    .buildRequest()
    .expand("eventMessage/event")
    .get();

```