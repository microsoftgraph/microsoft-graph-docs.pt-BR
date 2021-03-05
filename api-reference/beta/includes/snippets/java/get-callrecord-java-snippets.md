---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 85dd3787b4ba9d42d1f12cae63a2f0437221a4fb
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50472587"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

CallRecord callRecord = graphClient.communications().callRecords("{id}")
    .buildRequest()
    .get();

```