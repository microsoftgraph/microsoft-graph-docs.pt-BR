---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 41a26b16a1efeb2ace37c200cfe919bce71cb5d3
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50771915"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

IPrintTaskTriggerCollectionPage taskTriggers = graphClient.print().printers("{printerId}").taskTriggers()
    .buildRequest()
    .get();

```