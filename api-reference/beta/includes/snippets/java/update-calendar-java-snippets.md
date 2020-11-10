---
description: Arquivo gerado automaticamente. NÃO MODIFICAR
ms.openlocfilehash: 992024b3d5ae71be020e6bae6e24cde5684e05f7
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48960009"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

Calendar calendar = new Calendar();
calendar.name = "Social events";

graphClient.me().calendar()
    .buildRequest()
    .patch(calendar);

```